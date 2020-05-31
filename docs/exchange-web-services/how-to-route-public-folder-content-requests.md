---
title: Маршрутизация запросов содержимого общедоступных папок
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Все запросы к сведениям о общедоступных папках, включающих содержимое общедоступной папки, необходимо перенаправить на почтовый ящик общедоступных папок, содержащий контент для целевой папки. Чтобы перенаправить запросы в этот почтовый ящик, необходимо задать для заголовков X и AnchorMailbox и X Публикфолдермаилбокс определенные значения.
ms.openlocfilehash: 64fafecb9882b17a3394e54640df78f7aa180343
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354024"
---
# <a name="route-public-folder-content-requests"></a>Маршрутизация запросов содержимого общедоступных папок

Все запросы к сведениям о общедоступных папках, включающих содержимое общедоступной папки, необходимо перенаправить на почтовый ящик общедоступных папок, содержащий контент для целевой папки. Чтобы перенаправить запросы в этот почтовый ящик, необходимо задать для заголовков **x и AnchorMailbox** и **x публикфолдермаилбокс** определенные значения. 
  
В следующей таблице представлен обзор процесса.
  
**Общие сведения о общедоступной папке**

|Заголовок|Что нужно сделать?|Как это сделать?|
|:-----|:-----|:-----|
|**X — AnchorMailbox** <br/> |1. [значения x AnchorMailbox и x публикфолдеринформатион](how-to-route-public-folder-hierarchy-requests.md) для почтового ящика иерархии общедоступных папок.<br/><br/>2. идентификатор GUID почтового ящика общедоступных папок, который содержит содержимое почтового ящика, которое отправляется в службу автообнаружения.<br/><br/>  **Аутодисковерсмтпаддресс** в ответе обнаружение autodisover становится значением заголовка **X/AnchorMailbox** .  <br/> ![TODO](media/Ex15_PF_PFContent.png)| 1. Используйте пример кода, описанный в этой статье, который [реализует управляемый API EWS](#bk_determineguidewsma). Или [Используйте EWS](#bk_determineguidews) и преобразуйте результаты, чтобы получить GUID.<br/><br/>2. [сделайте запрос автообнаружения](#bk_makeautodrequest) с помощью идентификатора GUID и имени домена.<br/><br/>3. Используйте значение элемента **аутодисковерсмтпаддресс** , возвращенное в ответе автообнаружения для [заполнения значения заголовков](#bk_setheadervalues).  <br/> |
|**X — Публикфолдермаилбокс** <br/> |Ваши действия выполняются, значение X-Публикфолдермаилбокс совпадает со значением X-AnchorMailbox!  <br/> |У вас уже есть!  <br/> |
   
Определив значения заголовков, включите их [при создании запросов на содержимое общедоступных папок](#bk_setheadervalues).
  
Действия, описанные в этой статье, относятся к запросам содержимого общедоступных папок. Чтобы определить, является ли ваш запрос иерархией общедоступных папок или запроса содержимого, ознакомьтесь со статьей [Маршрутизация запросов](public-folder-access-with-ews-in-exchange.md#bk_routing)к общедоступным папкам.

<a name="bk_determineguidewsma"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>Определение GUID почтового ящика общедоступных папок с помощью управляемого API EWS


Чтобы определить GUID почтового ящика содержимого общедоступной папки, используйте следующий пример кода, который выполняет следующие действия: 
  
- Использует заголовки **x – AnchorMailbox** и **x – публикфолдеринформатион** , полученные с помощью [запроса иерархии маршрутизации общедоступных папок](how-to-route-public-folder-hierarchy-requests.md).
    
- Вызывает метод [Финдфолдерс](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) управляемого API EWS и включает запрос для свойства **PR_REPLICA_LIST** (0x66980102). 
    
**PR_REPLICA_LIST** значение определяет GUID почтового ящика общедоступных папок с содержимым папки. Свойство **PR_REPLICA_LIST** является массивом байтов, но приводится в качестве идентификатора GUID для этого сценария. GUID и имя домена сцепляются, чтобы сформировать адрес, на котором будет вызываться служба автообнаружения. 
  
В этом примере предполагается, что `service` это объект [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для пользователя почтового ящика, `PFHAnchorHeader` а `PFHMailboxHeader` также значения заголовков **x-AnchorMailbox** и **x-публикфолдермаилбокс** , а доменное доменное имя, используемое клиентом. 
  
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

Если вы получили сообщение об ошибке "не удалось выполнить запрос. Базовое соединение закрыто: не удалось установить отношение доверия для безопасного канала SSL/TLS ", вам потребуется [Добавить вызов метода обратного вызова проверки](how-to-validate-a-server-certificate-for-the-ews-managed-api.md). Заполнитель и комментарий для этого метода включены в пример кода.
  
Если GUID почтового ящика совпадает для всех общедоступных папок в корневом каталоге общедоступной папки, в примере указывается адрес, используемый при [вызове службы автообнаружения](#bk_makeautodrequest) в выходных данных консоли и в качестве возвращаемого значения. Если GUID почтового ящика не совпадает для всех общедоступных папок в корневом каталоге общедоступной папки, необходимо [выполнить запрос автообнаружения](#bk_makeautodrequest) на адрес, связанный с папкой в запросе содержимого. 

<a name="bk_determineguidews"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>Определение GUID почтового ящика общедоступных папок с помощью EWS

В приведенном ниже примере кода показано, как получить значение свойства **PR_REPLICA_LIST** (0x66980102) с помощью операции [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) для EWS. Для элемента [екстендедфиелдури](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) атрибут **пропертитаг** задается как десятичное значение (26264) свойства **PR_REPLICA_LIST** , а атрибут **propertyType** имеет значение **binary**.
  
Это также запрос XML, который отправляет управляемый API EWS при использовании метода **финдфолдерс** для [определения GUID почтового ящика общедоступных папок с помощью управляемого API EWS](#bk_determineguidewsma).
  
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

Сервер отвечает на запрос **FindFolder** с сообщением [финдфолдерреспонсе](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) , которое включает значение расширенного свойства **PR_REPLICA_LIST** . Обратите внимание, что значение свойства отображается в отклике EWS в виде строки в массиве байтов с кодировкой Base 64. Некоторые значения заголовков в отклике сокращаются для удобочитаемости. 
  
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

Чтобы использовать значение **PR_REPLICA_LIST** , возвращаемого в XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA = =, чтобы определить GUID почтового ящика, значение должно быть преобразовано в GUID в формате, аналогичном преобразовании значения в [пример кода управляемого API EWS](#bk_determineguidewsma). Затем GUID объединяется с доменным именем для создания SMTP-адреса, включенного в [запрос автообнаружения](#bk_makeautodrequest).
  
## <a name="make-an-autodiscover-request"></a>Выполнение запроса на автообнаружение
<a name="bk_makeautodrequest"> </a>

Используйте адрес, возвращенный `GetMailboxGuidAddress` методом для вызова службы автообнаружения. Мы рекомендуем использовать [Exchange 2013: получение параметров пользователя с помощью кода автообнаружения](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) для вызова службы автообнаружения, так как она упрощает процесс автообнаружения. В этом примере кода используются аргументы командной строки, приведенные в следующей таблице, для вызова службы автообнаружения POX для получения значения [аутодисковерсмтпаддресс](http://msdn.microsoft.com/en-us/library/office/dn750991%28v=exchg.150%29.aspx) , связанного с идентификатором GUID почтового ящика. 
  
|**Аргумент**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |Адрес, возвращенный `GetMailboxGuidAddress` методом в [определении GUID почтового ящика общедоступных папок](#bk_determineguidewsma).  <br/> |
|— Скипсоап  <br/> |Указывает, что требуются запросы автообнаружения POX.  <br/> |
|— Проверка подлинности Аусемаиладдресс  <br/> |Адрес электронной почты пользователя почтового ящика, используемый для проверки подлинности. При запуске примера вам будет предложено ввести пароль пользователя почтового ящика.  <br/> |
   
Например, аргументы командной строки должны выглядеть следующим образом:
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Где `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` — это адрес, возвращаемый методом **жетмаилбоксгуидаддресс** , и `sonyaf@contoso.com` является пользователем почтового ящика. 
  
При запуске **Exchange 2013: получение параметров пользователя с помощью службы автообнаружения** , последний ответ автообнаружения должен быть успешным и включать все параметры пользователя, связанные с идентификатором GUID почтового ящика. Сохраните параметр пользователя **аутодисковерсмтпаддресс** локально, как он будет использоваться на следующем шаге. 
  
Кроме того, если вы не хотите использовать **Exchange 2013: "получение параметров пользователя с помощью автообнаружения** ", вы можете получить параметр пользователя **аутодисковерсмтпаддресс** , [создав список конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md), а затем отправив следующий запрос автообнаружения POX для каждого URL-адреса, пока не будет получен успешный ответ.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автообнаружения: служба [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создание списка конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Задайте значения для заголовков X — AnchorMailbox и X Публикфолдермаилбокс
<a name="bk_setheadervalues"> </a>

Используя значение для **аутодисковерсмтпаддресс** , полученное в [запросе на автообнаружение](#bk_makeautodrequest), задайте значения для заголовков **x — AnchorMailbox** и **x публикфолдермаилбокс** в запросе содержимого общедоступных папок. 
  
Например, при вызове следующих методов или операций с помощью Аутодисковерсмтпаддресс NewPublicFolder@contoso.com включите следующие заголовки.
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**Вызовы общедоступных папок, требующие заголовков X Анкормаилбокс и X PublicFolder**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item. Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Элемент. Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовки с помощью управляемого API EWS, используйте метод [хттфеадерс. Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

В приведенном ниже коде показан запрос на получение [папки](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) с заголовком **x – AnchorMailbox** и **x – публикфолдермаилбокс** значениями, полученными в примерах, приведенных в этой статье. 
  
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
- [Создание списка конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

