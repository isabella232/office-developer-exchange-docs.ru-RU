---
title: Маршрутизация запросов к иерархии общедоступных папок
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Все запросы на сведения о общедоступных папках, которые требуют знаний о иерархии общедоступных папок, таких как перемещение, обновление, удаление или поиск общедоступных папок, должны быть переналожены в почтовый ящик иерархии общедоступных папок по умолчанию для данного пользователя. Чтобы отправить запросы в этот почтовый ящик, необходимо настроить заголовки X-AnchorMailbox и X-PublicFolderMailbox к определенным значениям, возвращенным службой автообнаружения.
ms.openlocfilehash: e86e1956db33b7ad8e654a22b980900b4f59dd87
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513124"
---
# <a name="route-public-folder-hierarchy-requests"></a>Маршрутизация запросов к иерархии общедоступных папок

Все запросы на сведения о общедоступных папках, которые требуют знаний о иерархии общедоступных папок, таких как перемещение, обновление, удаление или поиск общедоступных папок, должны быть переналожены в почтовый ящик иерархии общедоступных папок по умолчанию для данного пользователя. Чтобы отправить запросы в этот почтовый ящик, необходимо настроить заголовки **X-AnchorMailbox** и **X-PublicFolderMailbox** к определенным значениям, возвращенным службой автообнаружения. 
  
**Обзор общедоступных папок**

|Заголовок|Что мне нужно?|Как его получить?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |Значение [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) от ответа АВТОобнаружения [GetUserSettings,](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) которое становится значением заголовка **X-AnchorMailbox.**<br/><br/> ![Ответ X-AnchorMailbox](media/Ex15_PF_PFH_Anchor.png)| 1. Отправьте **запрос GetUserSetting** с адресом SMTP для почтового ящика пользователя.<br/><br/>2. Кэширование значения элемента **PublicFolderInformation,** возвращаемого службой автообнаружения. Это может быть кэшироваться из существующего вызова автооткрытия в коде, или нового вызова [EWS Managed API GetUserSettings](#bk_getpfinfoewsma) или запроса [SOAP GetUserSettings](#bk_getpfinfoews).  <br/><br/>3. Используйте **элемент PublicFolderInformation** для заполнения значения заголовка **X-AnchorMailbox.** Значение элемента **PublicFolderInformation** — smTP-адрес.  <br/> |
|**X-PublicFolderMailbox** <br/> |Значение [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) из ответа автообнаружения [POX,](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx)которое становится значением заголовка **X-PublicFolderMailbox.**<br/><br/> ![Ответ X-PublicFolderMailbox](media/Ex15_PF_PFH_PFMailbox.png)|1. Вызов службы автообнаружения [POX](#bk_makeautodrequest) с помощью адреса электронной почты **X-AnchorMailbox.**  <br/><br/>2. Используйте элемент **Server,** возвращаемый службой автообнаружения, для заполнения значения заголовка **X-PublicFolderMailbox.** Значение **X-PublicFolderMailbox** — smTP-адрес, в котором имя пользователя — GUID.  <br/> |

<br/>

После того как вы определите значения загона, включайте их при запросах иерархии [общедоступных папок.](#bk_setheadervalues)
  
Действия в этой статье специфичны для запросов иерархии общедоступных папок. Чтобы определить, является ли ваш запрос иерархией общедоступных папок или запросом контента, см. в рубке Запросы [общедоступных папок.](public-folder-access-with-ews-in-exchange.md#bk_routing)
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Определение значения заголовка X-AnchorMailbox с помощью управляемого API EWS
<a name="bk_getpfinfoewsma"> </a>

Чтобы получить значение [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) с помощью управляемого API EWS, можно кэширование значения элемента **PublicFolderInformation,** который возвращает существующий вызов службы автообнаружения, или сделать новый вызов. 
  
При новом вызове можно получить параметры пользователя с помощью ПАРАМЕТРОВ управляемых API пользователей [EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)Get с помощью управляемого [API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) в коде, а затем вызвать пример **метода GetUserSettings** с помощью следующего кода, который извлекает только значение элемента **PublicFolderInformation.** Включаем SMTP-адрес пользователя почтового ящика в качестве параметра ввода. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

После запуска кода на консоли отображаются следующие сведения:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Теперь, когда у вас есть значение **PublicFolderInformation,** включи его в качестве значения для заголовки X-AnchorMailbox во всех запросах иерархии общедоступных папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Определение значения заголовка X-AnchorMailbox с помощью SOAP
<a name="bk_getpfinfoews"> </a>

В следующем примере кода показано, как получить значение **PublicFolderInformation** с помощью [операции SOAP GetUserSettings.](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) Пользователь почтового ящика указан в элементе [Почтовый](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) ящик, а элемент [RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) ограничивает ответ на значение [PublicFolderInformation.](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

Ответ включает значение **PublicFolderInformation.** 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Теперь, когда у вас есть значение **PublicFolderInformation,** включи его в качестве значения для заголовки X-AnchorMailbox во всех запросах иерархии общедоступных папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Сделайте запрос автообнаружения для определения значения X-PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

Сделайте запрос автообнаружения с помощью SMTP-адреса **PublicFolderInformation,** который в настоящее время используется в качестве **значения X-AnchorMailbox.** Используйте [Exchange 2013 г.:](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) Получите параметры пользователя с образцом кода автооткрытия, чтобы вызвать службу автооткрытия, так как она упрощает процесс автооткрытия для вас. В этом примере кода аргументы командной строки, перечисленные в следующей таблице, используются для вызова службы автообнаружения POX на **smTP-адресе PublicFolderInformation.** 
  
|**Аргумент командной строки**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |Адрес **SMTP PublicFolderInformation.**  <br/> |
|-skipSOAP  <br/> | Используйте запросы автооткрытия POX для этого сценария.  <br/> |
|-authEmailAddress  <br/> |Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности. При запуске примера вам будет предложено ввести пароль пользователя почтового ящика.  <br/> |
   
Например, если SharedPublicFolder@contoso.com является smTP-адресом элемента **PublicFolderInformation,** а sonyaf@contoso.com — пользователем почтового ящика, аргументы командной строки должны выглядеть так. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

При запуске **Exchange 2013 г. Получить** параметры пользователя с помощью образца автообнаружа, последний ответ автообнаружать должен быть успешным и включить все параметры пользователя, связанные с GUID почтового ящика. Значение [Server,](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) связанное с элементом типа протокола [EXCH,](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) — это заглавное значение **X-PublicFolderInformation.** 
  
```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Кроме того, если вы не хотите использовать **Exchange 2013:** Получение параметров пользователя с образцом автооткрытия, вы можете получить значение **Server** путем создания списка конечных точек автооткрытия, а затем отправки следующего запроса автонаружение POX на каждый URL-адрес до получения успешного ответа. [](how-to-generate-a-list-of-autodiscover-endpoints.md) SharedPublicFolder@contoso.com является значением заголовка **X-PublicFolderMailbox.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автооткрытия см. в Exchange [autodiscover](how-to-generate-a-list-of-autodiscover-endpoints.md) [for Exchange,](autodiscover-for-exchange.md)сгенерировать список конечных точек автооткрытия и получить параметры пользователей из Exchange с помощью автооткрытия . [](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Настройка значений заголовок X-AnchorMailbox и X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

Использование значения smTP-адреса **PublicFolderInformation,** приобретенного в Определении значения заголовка [X-AnchorMailbox](#bk_getpfinfoewsma) с помощью управляемого API EWS или определения  значения заголовщика X-AnchorMailbox с помощью SOAP и значения Server, приобретенного в Запросе автообнаружения для определения значения [X-PublicFolderInformation,](#bk_makeautodrequest)установите значения заголовок **X-AnchorMailbox** и **X-PublicFolderMailbox** в запросе на содержимое общедоступных папок. [](#bk_getpfinfoews) 
  
Например, с учетом smTP-адреса **PublicFolderInformation** SharedPublicFolder@contoso.com  и значения сервера 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, включаем следующие заглавные главы при вызове на следующие методы или операции. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Вызовы общедоступных папок, которые требуют заглавных звонков X-AnchorMailbox и X-PublicFolder**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовок с помощью управляемого API EWS, используйте [метод HttpHeaders.Add.](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Например, в следующем коде показан запрос [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) с заголовщиком **X-AnchorMailbox** и **X-PublicFolderMailbox** к значениям, полученным в примерах этой статьи. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>См. также

- [Общих папок в Exchange доступ с EWS](public-folder-access-with-ews-in-exchange.md)    
- [Маршрутизация запросов к содержимому общедоступных папок](how-to-route-public-folder-content-requests.md)    
- [Получить параметры пользователя с помощью управляемого API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

