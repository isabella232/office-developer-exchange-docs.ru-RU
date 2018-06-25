---
title: Иерархия общедоступных папок маршрутизации запросов
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Все запросы для общих папок, которые требуют знания по иерархии общедоступных папок, такие как перемещение, обновление, удаление или поиск общих папок, должны перенаправляться в почтовый ящик иерархии общих папок по умолчанию для определенного пользователя. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки X AnchorMailbox и X-PublicFolderMailbox для определенного значения, возвращаемые службой автообнаружения.
ms.openlocfilehash: 983431864729edbb040a7206dae416d10bfb2b7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761116"
---
# <a name="route-public-folder-hierarchy-requests"></a>Иерархия общедоступных папок маршрутизации запросов

Все запросы для общих папок, которые требуют знания по иерархии общедоступных папок, такие как перемещение, обновление, удаление или поиск общих папок, должны перенаправляться в почтовый ящик иерархии общих папок по умолчанию для определенного пользователя. Чтобы перенаправлять запросы к почтовому ящику, необходимо задать заголовки **X AnchorMailbox** и **X-PublicFolderMailbox** для определенного значения, возвращаемые службой автообнаружения. 
  
**Обзор общих папок**

|Заголовок|Что нужно сделать?|Как его получить?|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |Значение [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) из ответа SOAP автообнаружения [GetUserSettings](http://msdn.microsoft.com/en-us/library/office/dd877096%28v=exchg.150%29.aspx) , которое будет значение заголовка **X-AnchorMailbox** .<br/><br/> ![ЗАДАЧ](media/Ex15_PF_PFH_Anchor.png)| 1. отправьте запрос **GetUserSetting** с SMTP-адрес почтового ящика пользователя.<br/><br/>2. кэширование значение элемента **PublicFolderInformation** , которое возвращает службы автообнаружения. Это может быть кэширования данных из существующей вызова службы автообнаружения в коде, или новый [звонок GetUserSettings управляемого API веб-служб Exchange](#bk_getpfinfoewsma) или [запрос GetUserSettings SOAP](#bk_getpfinfoews).  <br/><br/>3. Используйте элемент **PublicFolderInformation** для заполнения значение заголовка **X-AnchorMailbox** . Значение элемента **PublicFolderInformation** является адресом SMTP.  <br/> |
|**X-PublicFolderMailbox** <br/> |Значение [сервера](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) из [ответа POX автообнаружения](http://msdn.microsoft.com/en-us/library/bb204082%28v=exchg.150%29.aspx), который становится значением заголовка **X-PublicFolderMailbox** .<br/><br/> ![ЗАДАЧ](media/Ex15_PF_PFH_PFMailbox.png)|1. службы [вызова автообнаружения POX](#bk_makeautodrequest) , используя адрес электронной почты **X AnchorMailbox** .  <br/><br/>2. Используйте элемент **сервера** , возвращаемые службой автообнаружения для заполнения значение заголовка **X-PublicFolderMailbox** . Значение **X-PublicFolderMailbox** является адресом SMTP, где GUID — это имя пользователя.  <br/> |

<br/>

После определения значения заголовка включайте их [во время внесения запросы иерархии общих папок](#bk_setheadervalues).
  
Действия, описанные в этой статье относятся только к запросы иерархии общих папок. Чтобы определить, является ли запрос иерархии общедоступных папок или содержимого запроса, обратитесь к разделу [маршрутизации запросов общих папок](public-folder-access-with-ews-in-exchange.md#bk_routing).
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Определите значение заголовка X-AnchorMailbox с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_getpfinfoewsma"> </a>

Для получения значения [PublicFolderInformation (POX)](http://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) с помощью управляемого интерфейса API веб-служб Exchange, можно кэшировать значение элемента **PublicFolderInformation** , которое возвращает существующий вызов к службе автообнаружения или Новый звонок. 
  
Если вы выполняете Новый звонок, можно [получить параметры пользователя с помощью управляемого интерфейса API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[получить параметры пользователя с помощью управляемого интерфейса API веб-служб Exchange](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) для вашего кода, а затем вызвать **GetUserSettings** пример метода, используя следующий код, который извлекает только значение элемента **PublicFolderInformation** . Включите SMTP-адрес пользователя почтового ящика в качестве входного параметра. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

После выполнения кода, в консоли отображаются следующие сведения:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Теперь, когда значение **PublicFolderInformation** включите его в качестве значения для заголовка X-AnchorMailbox во всех запросах иерархии общих папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Определите значение заголовка X-AnchorMailbox, с помощью SOAP
<a name="bk_getpfinfoews"> </a>

В следующем примере кода показано, как получить значение **PublicFolderInformation** с помощью операции [GetUserSettings](http://msdn.microsoft.com/en-us/library/dd877096%28v=exchg.150%29.aspx) SOAP. Почтовый ящик пользователя задан в элементе [почтовых ящиков](http://msdn.microsoft.com/en-us/library/dd877076%28v=exchg.150%29.aspx) , а элемент [RequestedSettings](http://msdn.microsoft.com/en-us/library/office/dd877107%28v=exchg.150%29.aspx) ограничения в ответ на значение [PublicFolderInformation](http://msdn.microsoft.com/en-us/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
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

Ответ содержит значение **PublicFolderInformation** . 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Теперь, когда значение **PublicFolderInformation** включите его в качестве значения для заголовка X-AnchorMailbox во всех запросах иерархии общих папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Выполнения запроса службы автообнаружения для определения значения X PublicFolderInformation
<a name="bk_makeautodrequest"> </a>

С помощью **PublicFolderInformation** SMTP-адрес, который теперь используется как значение **X-AnchorMailbox** выполнения запроса службы автообнаружения. Использование [Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) пример кода для вызова службы автообнаружения, так как он оптимизирует процесса автообнаружения для вас. В этом примере код использует аргументы командной строки, указанные в следующей таблице для вызова службы автообнаружения POX на **PublicFolderInformation** SMTP-адрес. 
  
|**Аргумент командной строки**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |Адрес **PublicFolderInformation** SMTP.  <br/> |
|-skipSOAP  <br/> | Использование запросов POX автообнаружения для этого сценария.  <br/> |
|-проверкой подлинности на основе authEmailAddress  <br/> |Адрес электронной почты пользователя почтового ящика, который используется для проверки подлинности. Будет предложено ввести пароль пользователя почтового ящика, при выполнении примера.  <br/> |
   
Например при SharedPublicFolder@contoso.com SMTP-адрес элемента, **PublicFolderInformation** и sonyaf@contoso.com — пользователь, почтовый ящик, аргументы командной строки должен выглядеть следующим образом. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

При выполнении **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, последний ответ автообнаружения должен быть успешные и включают все пользовательские параметры, связанные с GUID почтового ящика. Значение [сервера](http://msdn.microsoft.com/en-us/library/bb204084%28v=exchg.150%29.aspx) , связанные с помощью [протокола](http://msdn.microsoft.com/en-us/library/bb204278%28v=exchg.150%29.aspx)EXCH[Тип](http://msdn.microsoft.com/en-us/library/office/bb204223%28v=exchg.150%29.aspx) элемента — значение заголовка **X-PublicFolderInformation** . 
  
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

Кроме того Если вы не хотите использовать **Exchange 2013: Получение параметров пользователя с помощью службы автообнаружения** образец, можно получить значение **Server** [Создание списка конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md), а затем Отправка следующие POX автообнаружения запрос для каждого URL-адреса до получения успешного ответа. SharedPublicFolder@contoso.com — это значение заголовка **X-PublicFolderMailbox** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автообнаружения можно [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создать список конечных точек службы автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Задайте значения заголовков X AnchorMailbox и X-PublicFolderMailbox
<a name="bk_setheadervalues"> </a>

С использованием значения адреса **PublicFolderInformation** SMTP, полученные в [Определение значение заголовка X-AnchorMailbox с помощью управляемого интерфейса API веб-служб Exchange](#bk_getpfinfoewsma) или [Определите значение заголовка X-AnchorMailbox, с помощью SOAP](#bk_getpfinfoews) и **сервера **значение приобретенного в [выполнения запроса службы автообнаружения для определения значения X PublicFolderInformation](#bk_makeautodrequest), задайте значения **X AnchorMailbox** и **X-PublicFolderMailbox** заголовков в вашем запросе контента общей папки. 
  
Например учитывая **PublicFolderInformation** SMTP-адрес SharedPublicFolder@contoso.com и **сервера** значение 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, включены следующие заголовки при выполнении вызовов следующим методы или операции. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Вызовы общих папок, которые требуют X AnchorMailbox и X-PublicFolder заголовков**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](http://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовки с помощью управляемого интерфейса API веб-служб Exchange, используйте метод [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Например в следующем коде показан запрос [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) с заголовка **X-AnchorMailbox** и **X PublicFolderMailbox** , значения, полученные на примерах в этой статье. 
  
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
- [Маршрутизация запросов контента общей папки](how-to-route-public-folder-content-requests.md)    
- [Получение параметров пользователя с помощью управляемого интерфейса API веб-служб Exchange](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

