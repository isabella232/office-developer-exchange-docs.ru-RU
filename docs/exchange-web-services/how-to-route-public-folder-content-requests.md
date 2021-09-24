---
title: Маршрутизация запросов к содержимому общедоступных папок
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Все запросы на сведения о общедоступных папках, которые включают содержимое общедоступных папок, должны быть направлены в почтовый ящик общедоступных папок, в который содержится содержимое целевой папки. Чтобы отправить запросы в этот почтовый ящик, необходимо настроить заголовки X-AnchorMailbox и X-PublicFolderMailbox к определенным значениям.
ms.openlocfilehash: d5a066a63d9bc3b48c41473545343125538d856b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521104"
---
# <a name="route-public-folder-content-requests"></a>Маршрутизация запросов к содержимому общедоступных папок

Все запросы на сведения о общедоступных папках, которые включают содержимое общедоступных папок, должны быть направлены в почтовый ящик общедоступных папок, в который содержится содержимое целевой папки. Чтобы отправить запросы в этот почтовый ящик, необходимо настроить заголовки **X-AnchorMailbox** и **X-PublicFolderMailbox** к определенным значениям. 
  
В следующей таблице представлен обзор процесса:
  
**Обзор общедоступных папок**

|Заголовок|Что мне нужно?|Как его получить?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |1. [Значения X-AnchorMailbox и X-PublicFolderInformation ](how-to-route-public-folder-hierarchy-requests.md) для почтового ящика иерархии общедоступных папок.<br/><br/>2. GUID почтового ящика общедоступных папок, который содержит содержимое почтовых ящиков, отправляется в службу автообнаружания.<br/><br/>  **АвтообнаруженияSMTPAddress** в ответе автообнаружения становится значением заголовка **X-AnchorMailbox.**  <br/> ![TODO](media/Ex15_PF_PFContent.png)| 1. Используйте пример кода в этой статье, которая реализует [управляемый API EWS](#bk_determineguidewsma). Или [используйте EWS и](#bk_determineguidews) преобразуйте результаты для получения GUID.<br/><br/>2. [Сделайте запрос автооткрытия](#bk_makeautodrequest) с помощью GUID плюс доменное имя.<br/><br/>3. Используйте значение элемента **AutoDiscoverSMTPAddress,** возвращаемого в ответе автооткрытия, чтобы заполнить значение [заголовок.](#bk_setheadervalues)  <br/> |
|**X-PublicFolderMailbox** <br/> |Ваша работа сделана, значение X-PublicFolderMailbox такое же, как и значение X-AnchorMailbox!  <br/> |У вас уже есть!  <br/> |
   
После того, как вы определите значения загона, включайте их при запросах содержимого [общедоступных папок.](#bk_setheadervalues)
  
Действия в этой статье являются специфическими для запросов контента общедоступных папок. Чтобы определить, является ли ваш запрос иерархией общедоступных папок или запросом контента, см. в рубке Запросы [общедоступных папок.](public-folder-access-with-ews-in-exchange.md#bk_routing)

<a name="bk_determineguidewsma"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>Определение GUID почтового ящика общедоступных папок с помощью управляемого API EWS


Чтобы определить GUID почтового ящика контента общедоступных папок, используйте следующий пример кода, который делает следующее: 
  
- Использует **заглавы X-AnchorMailbox** и **X-PublicFolderInformation,** полученные путем маршрутизации запросов иерархии общедоступных [папок.](how-to-route-public-folder-hierarchy-requests.md)
    
- Вызывает метод [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) управляемого API EWS и  включает запрос на свойство PR_REPLICA_LIST (0x66980102) 
    
Значение **PR_REPLICA_LIST** определяет GUID почтового ящика почтового ящика общедоступных папок, который имеет содержимое для папки. Свойство **PR_REPLICA_LIST** является массивом byte, но отбрасована в качестве GUID для этого сценария. GUID и доменное имя согласуются, чтобы сформировать адрес, по которому можно вызвать автонаружение. 
  
В этом примере предполагается, что это объект ExchangeService для пользователя почтового ящика, а также значения заглавных окей `service` [](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) `PFHAnchorHeader` `PFHMailboxHeader` **X-AnchorMailbox** и **X-PublicFolderMailbox,** а домен — это доменное имя, используемое клиентом. 
  
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

Если вы получили ошибку "Запрос не удалось. Базовая связь была закрыта: не удалось установить доверительные отношения для безопасного канала SSL/TLS", необходимо добавить вызов в метод проверки [вызова.](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) В пример кода включено местообладатель и комментарий к этому методу.
  
Если GUID почтовых ящиков является одинаковым для всех общедоступных папок в корне общедоступных папок, в примере указывается адрес, который следует использовать при вызове автообнаружания в выходной консоли и в качестве возвращаемого значения. [](#bk_makeautodrequest) Если GUID почтовых ящиков не является одинаковым для всех общедоступных [](#bk_makeautodrequest) папок в корне общедоступных папок, необходимо сделать запрос автообнаружания по адресу, связанному с папкой в запросе на контент. 

<a name="bk_determineguidews"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>Определение GUID почтового ящика общедоступных папок с помощью EWS

В следующем примере кода показано, как получить значение свойства PR_REPLICA_LIST **(0x66980102)** с помощью операции EWS [FindFolder.](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) Для элемента [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) атрибут **PropertyTag** засмеялся десятичным значением (26264) свойства PR_REPLICA_LIST, а атрибут **PropertyType** — двоичным **.** 
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindFolders** для определения GUID почтового ящика общедоступных папок с помощью управляемого [API EWS.](#bk_determineguidewsma)
  
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

Сервер отвечает на запрос **FindFolder** [сообщением FindFolderResponse,](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) которое включает значение PR_REPLICA_LIST **расширенного** свойства. Обратите внимание, что значение свойства отображается в ответе EWS в виде строки в массиве byte с кодом base-64. Некоторые значения загона в ответе сокращаются для читаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
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

Чтобы использовать значение PR_REPLICA_LIST,  возвращенного в XML, MWVjMmEyMzYtZWWQ5My00Zjg4LWI5YzYtNlNnjNmYRhYTQ0AA=== для определения GUID почтового ящика, значение должно быть преобразовано в GUID в формате, аналогичном преобразованию значения в примере управляемого [API EWS](#bk_determineguidewsma). Затем GUID согласуется с доменным именем для создания SMTP-адреса, который входит в запрос [автонаружения.](#bk_makeautodrequest)
  
## <a name="make-an-autodiscover-request"></a>Сделать запрос на автонаружие
<a name="bk_makeautodrequest"> </a>

Используйте адрес, возвращенный  `GetMailboxGuidAddress` методом, чтобы вызвать автонаружие. Рекомендуется использовать Exchange [2013 г. Для](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) вызова службы автооткрытия параметров пользователя с образцом кода автооткрытия необходимо вызвать службу автооткрытия, так как она упрощает процесс автооткрытия для вас. Этот пример кода использует аргументы командной строки, перечисленные в следующей таблице, чтобы вызвать службу автообнаружения POX для получения значения [AutoDiscoverSMTPAddress,](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) связанного с GUID почтового ящика. 

  
|**Аргумент**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |Адрес, возвращенный методом в Определении GUID почтового ящика `GetMailboxGuidAddress` [общедоступных папок.](#bk_determineguidewsma)  <br/> |
|-skipSOAP  <br/> |Указывает, что требуются запросы на автоматическое открытие POX.  <br/> |
|-authEmailAddress  <br/> |Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности. При запуске примера вам будет предложено ввести пароль пользователя почтового ящика.  <br/> |
   
Например, аргументы командной строки должны выглядеть так:
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

Где `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` находится адрес, возвращаемый методом **GetMailboxGuidAddress,** и `sonyaf@contoso.com` является пользователем почтового ящика. 
  
При запуске **Exchange 2013 г. Получить** параметры пользователя с помощью образца автообнаружа, последний ответ автообнаружать должен быть успешным и включить все параметры пользователя, связанные с GUID почтового ящика. Сохраните **параметр пользователя AutoDiscoverSMTPAddress** локально, так как вы будете использовать его на следующем шаге. 
  
Кроме того, если вы не хотите использовать **Exchange 2013:** Получение параметров пользователя с помощью примера автооткрытия, вы можете получить параметр пользователя **AutoDiscoverSMTPAddress,** создавая список конечных точек автооткрытия, [](how-to-generate-a-list-of-autodiscover-endpoints.md)а затем отправляя следующий запрос автооткрытия POX на каждый URL-адрес до получения успешного ответа.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автооткрытия см. в Exchange [autodiscover](how-to-generate-a-list-of-autodiscover-endpoints.md) [for Exchange,](autodiscover-for-exchange.md)сгенерировать список конечных точек автооткрытия и получить параметры пользователей из Exchange с помощью автооткрытия . [](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Настройка значений заголовок X-AnchorMailbox и X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Используя значение для автообнаруженияSMTPAddress, приобретенного в запросе Автообнаружения, установите значения заглавных разделов **X-AnchorMailbox** и **X-PublicFolderMailbox** в запросе содержимого общедоступных папок.  [](#bk_makeautodrequest) 
  
Например, если вы предоставляете автооткрывателиSMTPAddress NewPublicFolder@contoso.com, включим следующие заголовки при вызове на следующие методы или операции.
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**Вызовы общедоступных папок, для звонков в которые требуются заголовки X-AncorMailbox и X-PublicFolder**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовок с помощью управляемого API EWS, используйте [метод HttpHeaders.Add.](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

В следующем коде показан запрос [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) с заголовщиком **X-AnchorMailbox** и **X-PublicFolderMailbox,** задатким значениям, полученным в примерах этой статьи. 
  
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
- [Автообнаружение в Exchange](autodiscover-for-exchange.md)    
- [Создание списка конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  
