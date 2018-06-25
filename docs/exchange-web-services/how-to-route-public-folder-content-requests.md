---
title: Маршрутизация запросов контента общей папки
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Все запросы для общих папок, включающих содержимое общих папок необходимость направляться в почтовый ящик общедоступных папок, в которой содержится контент для целевой папке. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки X AnchorMailbox и X-PublicFolderMailbox для определенного значения.
ms.openlocfilehash: ad36c1526a24d815ec690879d633774d429ed36c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761123"
---
# <a name="route-public-folder-content-requests"></a>Маршрутизация запросов контента общей папки

Все запросы для общих папок, включающих содержимое общих папок необходимость направляться в почтовый ящик общедоступных папок, в которой содержится контент для целевой папке. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки **X AnchorMailbox** и **X-PublicFolderMailbox** для определенного значения. 
  
Следующая таблица содержит обзор процесса:
  
**Обзор общих папок**

|Заголовок|Что нужно сделать?|Как его получить?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |1. [X-AnchorMailbox и X PublicFolderInformation значения](how-to-route-public-folder-hierarchy-requests.md) для почтового ящика иерархии общедоступных папок.<br/><br/>2. идентификатор GUID почтового ящика общедоступных папок с содержимым почтового ящика, которое передается для службы автообнаружения.<br/><br/>  **AutoDiscoverSMTPAddress** в ответе Autodisover становится значение заголовка **X-AnchorMailbox** .  <br/> ![ЗАДАЧ](media/Ex15_PF_PFContent.png)| 1. Используйте в примере кода в этой статье, который [реализует управляемый API веб-служб Exchange](#bk_determineguidewsma). Или [Используйте веб-служб Exchange](#bk_determineguidews) и преобразования результатов, чтобы получить идентификатор GUID.<br/><br/>2. [выполнения запроса автоматического обнаружения](#bk_makeautodrequest) с помощью идентификатора GUID, а также имя домена.<br/><br/>3. Используйте значение элемента **AutoDiscoverSMTPAddress** , возвращаемого в ответе автообнаружения для [заполнения значения заголовков](#bk_setheadervalues).  <br/> |
|**X-PublicFolderMailbox** <br/> |На работу, значение X-PublicFolderMailbox — то же, что значение X-AnchorMailbox!  <br/> |У вас уже есть его!  <br/> |
   
После определения значения заголовка включайте их [во время внесения запросов контента общей папки](#bk_setheadervalues).
  
Действия, описанные в этой статье относятся только к запросов контента общей папки. Чтобы определить, является ли запрос иерархии общедоступных папок или содержимого запроса, обратитесь к разделу [маршрутизации запросов общих папок](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>Определите идентификатор GUID почтового ящика общедоступных папок с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_determineguidewsma"> </a>

Для определения идентификатора GUID почтового ящика содержимого общей папки, используйте приведенный ниже код, который выполняет следующие: 
  
- Используется в заголовках **X-AnchorMailbox** и **X PublicFolderInformation** загрузки [маршрутизации](how-to-route-public-folder-hierarchy-requests.md)запросов иерархии общих папок.
    
- Вызывает метод управляемый API EWS [FindFolders](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) и включает в себя запрос для свойства **PR_REPLICA_LIST** (0x66980102) 
    
Значение **PR_REPLICA_LIST** определяет идентификатор GUID почтового ящика общей папки, который содержит содержимое папки почтового ящика. Свойство **PR_REPLICA_LIST** является массив байтов, но приводится как код GUID для этого сценария. Идентификатор GUID и имя домена объединяется адрес, на котором для вызова службы автообнаружения. 
  
В этом примере предполагается, что `service` — это объект [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для пользователя почтового ящика, `PFHAnchorHeader` и `PFHMailboxHeader` значения заголовков **X AnchorMailbox** и **X-PublicFolderMailbox** и домен — это имя домена, используемого клиент. 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

Если ошибка «не удалось выполнить запрос. Базовое соединение закрыто: не удается установить отношение доверия для безопасного канала SSL/TLS», необходимо [Добавить вызов метода обратного вызова проверки](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). В примере кода включается заполнитель и комментарий для этого метода.
  
Если GUID почтового ящика является общим для всех общих папок в корне общей папки, в примере указывается адрес для [вызова службы автообнаружения](#bk_makeautodrequest) в консоли вывода и как возвращаемое значение. Идентификатор GUID почтового ящика не является общим для всех общих папок в корне общей папки, требуется ли [выполнения запроса службы автообнаружения](#bk_makeautodrequest) на адрес, сопоставленный с папкой в вашем запросе контента. 
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>Определите идентификатор GUID почтового ящика общедоступных папок с помощью веб-служб Exchange
<a name="bk_determineguidews"> </a>

В следующем примере кода показано, как получить значение свойства **PR_REPLICA_LIST** (0x66980102) с помощью веб-служб Exchange [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) операции. Для элемента [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) атрибута **PropertyTag** указывается десятичное значение свойства **PR_REPLICA_LIST** (26264), атрибут **PropertyType** задано значение **двоичный**.
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindFolders** , чтобы [определить GUID почтового ящика общедоступных папок с помощью управляемого интерфейса API веб-служб Exchange](#bk_determineguidewsma).
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **FindFolder** [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) сообщение, содержащее значение **PR_REPLICA_LIST** расширенные свойства. Обратите внимание, что отображается значение свойства ответа веб-служб Exchange как строку формата base 64 закодированный массив байтов. Некоторые значения заголовка в ответе сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

Чтобы использовать значение **PR_REPLICA_LIST** возвращается в XML-КОДЕ MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA ==, чтобы определить GUID почтового ящика, значение должны быть преобразованы в идентификатор GUID в формате, аналогичном как значение преобразуется в [Пример кода управляемый API веб-служб Exchange](#bk_determineguidewsma). Идентификатор GUID затем соединяется с именем домена для создания SMTP-адрес, который включен в [запрос автообнаружения](#bk_makeautodrequest).
  
## <a name="make-an-autodiscover-request"></a>Для выполнения запроса службы автообнаружения
<a name="bk_makeautodrequest"> </a>

Используйте адрес, возвращенный `GetMailboxGuidAddress` метод, вызываемый службы автообнаружения. Мы рекомендуем использовать [Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) пример кода для вызова службы автообнаружения, так как он оптимизирует процесса автообнаружения для вас. В этом примере код использует аргументы командной строки, указанные в следующей таблице для вызова службы автообнаружения POX для извлечения значения [AutoDiscoverSMTPAddress](http://msdn.microsoft.com/en-us/library/office/dn750991%28v=exchg.150%29.aspx) , связанный с GUID почтового ящика. 
  
|**Аргумент**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |Адрес, возвращенный `GetMailboxGuidAddress` метода в [Определение GUID почтового ящика общедоступных папок](http://msdn.microsoft.com/library/bk_determineguidewsma.aspx).  <br/> |
|-skipSOAP  <br/> |Указывает, что запросов автообнаружения POX требуются.  <br/> |
|-проверкой подлинности на основе authEmailAddress  <br/> |Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности. Будет предложено ввести пароль пользователя почтового ящика, при выполнении примера.  <br/> |
   
Например аргументы командной строки должна выглядеть следующим образом:
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Где `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` — это адрес, возвращенный методом **GetMailboxGuidAddress** и `sonyaf@contoso.com` — пользователь, почтовый ящик. 
  
При выполнении **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, последний ответ автообнаружения должен быть успешные и включают все пользовательские параметры, связанные с GUID почтового ящика. Сохранить **AutoDiscoverSMTPAddress** пользователя, задание локально, как она будет использоваться на следующем этапе. 
  
Кроме того Если вы не хотите использовать **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, вы получаете пользователя **AutoDiscoverSMTPAddress** параметру, [создав список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и затем Отправка следующие Запрос автообнаружения POX для каждого URL-адреса до получения успешного ответа.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автообнаружения можно [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создать список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Задайте значения заголовков X AnchorMailbox и X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

С использованием значения для **AutoDiscoverSMTPAddress** , полученные в [выполнения запроса службы автообнаружения](#bk_makeautodrequest), задайте значения заголовков **X AnchorMailbox** и **X-PublicFolderMailbox** в вашем запросе контента общей папки. 
  
Например учитывая AutoDiscoverSMTPAddress NewPublicFolder@contoso.com, включают следующие заголовки при вызове следующих методов или операции.
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**Вызовы общих папок, которые требуют X AncorMailbox и X-PublicFolder заголовков**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовки с помощью управляемого интерфейса API веб-служб Exchange, используйте метод [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

В следующем коде показан запрос [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) с заголовка **X-AnchorMailbox** и **X PublicFolderMailbox** , значения, полученные на примерах в этой статье. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также

- [Общих папок в Exchange доступ с EWS](public-folder-access-with-ews-in-exchange.md)    
- [Автообнаружение для Exchange](autodiscover-for-exchange.md)    
- [Создать список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

