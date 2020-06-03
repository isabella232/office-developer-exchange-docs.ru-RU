---
title: Маршрутизация запросов иерархии общедоступных папок
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: Все запросы для сведений о общедоступных папках, которым требуется знание иерархии общедоступных папок, например перемещение, обновление, удаление или поиск общедоступных папок, необходимо перенаправить на почтовый ящик иерархии общедоступных папок по умолчанию для данного пользователя. Чтобы перенаправить запросы в этот почтовый ящик, необходимо установить для заголовков X и AnchorMailbox и X Публикфолдермаилбокс конкретные значения, возвращаемые службой автообнаружения.
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455703"
---
# <a name="route-public-folder-hierarchy-requests"></a>Маршрутизация запросов иерархии общедоступных папок

Все запросы для сведений о общедоступных папках, которым требуется знание иерархии общедоступных папок, например перемещение, обновление, удаление или поиск общедоступных папок, необходимо перенаправить на почтовый ящик иерархии общедоступных папок по умолчанию для данного пользователя. Чтобы перенаправить запросы в этот почтовый ящик, необходимо установить для заголовков **x и AnchorMailbox** и **x публикфолдермаилбокс** конкретные значения, возвращаемые службой автообнаружения. 
  
**Общие сведения о общедоступных папках**

|Заголовок|Что нужно сделать?|Как это сделать?|
|:-----|:-----|:-----|
|**X — AnchorMailbox** <br/> |Значение [публикфолдеринформатион](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) из ответа SOAP службы автообнаружения [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) , которое становится значением заголовка **X/AnchorMailbox** .<br/><br/> ![TODO](media/Ex15_PF_PFH_Anchor.png)| 1. Отправьте запрос **жетусерсеттинг** с SMTP-адресом для почтового ящика пользователя.<br/><br/>2. кэширование значения элемента **публикфолдеринформатион** , возвращаемого службой автообнаружения. Это может быть кэшировано из существующего вызова автообнаружения в коде или с помощью нового [вызова GetUserSettings управляемого API EWS](#bk_getpfinfoewsma) или [запроса GetUserSettings SOAP](#bk_getpfinfoews).  <br/><br/>3. Используйте элемент **публикфолдеринформатион** для заполнения значения заголовка **X – AnchorMailbox** . Значение элемента **публикфолдеринформатион** — SMTP-адрес.  <br/> |
|**X — Публикфолдермаилбокс** <br/> |Значение [сервера](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) из [отклика автообнаружения POX](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx), которое становится значением заголовка **X – публикфолдермаилбокс** .<br/><br/> ![TODO](media/Ex15_PF_PFH_PFMailbox.png)|1. [вызовите службу АВТООБНАРУЖЕНИЯ POX](#bk_makeautodrequest) , используя адрес электронной почты **X – AnchorMailbox** .  <br/><br/>2. Используйте **Серверный** элемент, возвращенный службой автообнаружения, для заполнения значения заголовка **X – публикфолдермаилбокс** . Значение **X-публикфолдермаилбокс** — это SMTP-адрес, где имя пользователя — GUID.  <br/> |

<br/>

После определения значений заголовков включите их при выполнении [запросов иерархии общедоступных папок](#bk_setheadervalues).
  
Действия, описанные в этой статье, относятся к запросам иерархии общедоступных папок. Чтобы определить, является ли ваш запрос иерархией общедоступных папок или запроса содержимого, ознакомьтесь со статьей [Маршрутизация запросов](public-folder-access-with-ews-in-exchange.md#bk_routing)к общедоступным папкам.
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>Определение значения заголовка X-AnchorMailbox с помощью управляемого API EWS
<a name="bk_getpfinfoewsma"> </a>

Чтобы получить значение [публикфолдеринформатион (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) с помощью управляемого API EWS, можно кэшировать значение элемента **публикфолдеринформатион** , который возвращает существующий вызов службы автообнаружения, или создать новый вызов. 
  
Если вы создаете новый звонок, вы можете [получить параметры пользователя с помощью управляемого API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed), чтобы[получить параметры пользователя с помощью управляемого API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed) для кода, а затем вызвать метод **GetUserSettings** , используя следующий код, который извлекает только значение элемента **публикфолдеринформатион** . Включите SMTP-адрес пользователя почтового ящика в качестве входного параметра. 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

После выполнения кода на консоли отображаются следующие сведения:
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

Теперь, когда у вас есть значение **публикфолдеринформатион** , включите его в качестве значения для заголовка X – AnchorMailbox во всех запросах иерархии общедоступных папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>Определение значения заголовка X – AnchorMailbox с помощью SOAP
<a name="bk_getpfinfoews"> </a>

В приведенном ниже примере кода показано, как получить значение **публикфолдеринформатион** с помощью операции SOAP [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) . Пользователь почтового ящика указан в элементе [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) , а элемент [рекуестедсеттингс](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) — ограничено значением [публикфолдеринформатион](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
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

Ответ включает значение **публикфолдеринформатион** . 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

Теперь, когда у вас есть значение **публикфолдеринформатион** , включите его в качестве значения для заголовка X – AnchorMailbox во всех запросах иерархии общедоступных папок. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>Выполнение запроса автообнаружения для определения значения X Публикфолдеринформатион
<a name="bk_makeautodrequest"> </a>

Выполните запрос автообнаружения с помощью SMTP-адреса **публикфолдеринформатион** , который теперь используется в качестве значения **X-AnchorMailbox** . Используйте [сервер Exchange 2013: получение параметров пользователя с помощью кода автообнаружения](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) для вызова службы автообнаружения, так как она упрощает процесс автообнаружения. В этом примере кода используются аргументы командной строки, приведенные в следующей таблице, для вызова службы автообнаружения POX на SMTP-адресе **публикфолдеринформатион** . 
  
|**Аргумент командной строки**|**Описание**|
|:-----|:-----|
|emailAddress  <br/> |SMTP-адрес **публикфолдеринформатион** .  <br/> |
|— Скипсоап  <br/> | Используйте запросы автообнаружения POX для этого сценария.  <br/> |
|— Проверка подлинности Аусемаиладдресс  <br/> |Адрес электронной почты пользователя почтового ящика, используемый для проверки подлинности. При запуске примера вам будет предложено ввести пароль пользователя почтового ящика.  <br/> |
   
Например, если SharedPublicFolder@contoso.com — SMTP-адрес элемента **публикфолдеринформатион** , а sonyaf@contoso.com — пользователь почтового ящика, аргументы командной строки должны выглядеть следующим образом. 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

При запуске **Exchange 2013: получение параметров пользователя с помощью службы автообнаружения** , последний ответ автообнаружения должен быть успешным и включать все параметры пользователя, связанные с идентификатором GUID почтового ящика. Значение [сервера](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) , связанное с элементом [Protocol](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[тип](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) протокола, — это значение заголовка **X-публикфолдеринформатион** . 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

Кроме того, если вы не хотите использовать **Exchange 2013: получение параметров пользователя с помощью службы автообнаружения** , можно получить значение **сервера** , создав [список конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и затем отправив следующий запрос автообнаружения POX для каждого URL-адреса, пока не будет получен успешный ответ. SharedPublicFolder@contoso.com — значение заголовка **X-публикфолдермаилбокс** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

Дополнительные сведения о процессе автообнаружения: служба [автообнаружения для Exchange](autodiscover-for-exchange.md), [Создание списка конечных точек автообнаружения](how-to-generate-a-list-of-autodiscover-endpoints.md)и [Получение параметров пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>Задайте значения для заголовков X — AnchorMailbox и X Публикфолдермаилбокс
<a name="bk_setheadervalues"> </a>

С помощью значения SMTP-адреса **публикфолдеринформатион** , полученного в разделе [Определение значения заголовка x-AnchorMailbox с помощью управляемого API EWS](#bk_getpfinfoewsma) или [определения значения заголовка x-AnchorMailbox с помощью SOAP](#bk_getpfinfoews) и значения **сервера** , полученного в запросе на [обнаружение для определения значения x-публикфолдеринформатион](#bk_makeautodrequest), задайте значения **x-AnchorMailbox** и **x-публикфолдермаилбокс** в запросе содержимого общедоступной папки. 
  
Например, если указан SMTP-адрес **публикфолдеринформатион** SharedPublicFolder@contoso.com и значение **сервера** 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com, при вызове следующих методов или операций необходимо включить следующие заголовки. 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**Вызовы общедоступных папок, требующие заголовков X AnchorMailbox и X PublicFolder**

|**Методы управляемого API EWS**|**Операции EWS**|
|:-----|:-----|
|[Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Папка. Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
Чтобы добавить эти заголовки с помощью управляемого API EWS, используйте метод [хттфеадерс. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) . 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

Например, в приведенном ниже коде показан запрос [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) с заголовком **x – AnchorMailbox** и **x – публикфолдермаилбокс** , для которых заданы значения, полученные в примерах, приведенных в этой статье. 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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
- [Маршрутизация запросов содержимого общедоступных папок](how-to-route-public-folder-content-requests.md)    
- [Получение параметров пользователя с помощью управляемого API EWS](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

