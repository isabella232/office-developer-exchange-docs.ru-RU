---
title: Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Узнайте о поддержке сходства между группой подписок и сервера почтовых ящиков.
ms.openlocfilehash: 7cfbfb5cc19e092c37e3d48a7fcc4f27023516e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761030"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange

Узнайте о поддержке сходства между группой подписок и сервера почтовых ящиков.
  
Сходство — связь последовательность сообщений, запрос и ответ с определенного сервера почтовых ящиков. Для большинства функций в Exchange сходства обрабатывается на сервере. Уведомления, однако, исключение. Клиент несет ответственность за обеспечение соответствия с сервером почтовых ящиков для подписки на уведомления. В этом сходства позволяет подсистемы балансировки нагрузки и серверы клиентского доступа между клиентом и сервера для подписки на уведомления о маршрутизации и связанных с ними запросов на сервере почтовых ящиков, который поддерживает подписки. Без сходства запрос могут быть маршрутизированы на другой сервер почтовых ящиков, которая не включает клиентских подписок, которые могут вызвать ошибку [ErrorSubscriptionNotFound](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) должно быть возвращено. 
  
## <a name="how-is-affinity-maintained"></a>Как поддерживается сходства?
<a name="bk_howmaintained"> </a>

Сходство в Exchange — на основе файлов cookie. Клиент инициирует создание файла cookie, включая определенных заголовков в запрос подписки, а затем ответа подписки содержит файл cookie. Затем клиент передает этот файл в последующие запросы, чтобы убедиться, что запрос перенаправляется в правом сервера почтовых ящиков.
  
В частности сходства в Exchange обрабатывается следующее: 
  
- X-AnchorMailbox — Заголовок HTTP, который включен в запрос начальной подписки. Он определяет первый почтовых ящиков в группе почтовых ящиков, которые совместно использовать сходство на одном сервере почтовых ящиков.
    
- X-PreferServerAffinity — Заголовка HTTP, который включен в запрос начальной подписки с заголовка X-AnchorMailbox и задано значение true, чтобы указать, что клиент запрашивает обслуживать сходства с сервера почтовых ящиков.
    
- X-BackEndOverrideCookie — Файл cookie, включенных в ответ начальной подписки и содержит файл cookie, балансировки нагрузки и сервера клиентского доступа для маршрутизировать последующие запросы на том же сервере почтовых ящиков.
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>Как поддерживать сходства с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange?
<a name="bk_howdoimaintain"> </a>

Можно использовать те же действия для обеспечения соответствия для подписки на несколько почтовых ящиков и их серверах почтовых ящиков, независимо от того, используется ли потоковая передача, запросу или push-уведомлений, и независимо от того, является ли целевой локальную систему Exchange server или Exchange Online.
  
1. Для каждого почтового ящика, [вызова службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и получение параметров GroupingInformation и ExternalEwsUrl пользователя. Для службы автообнаружения SOAP используйте элемент [параметра](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) и для службы автообнаружения POX, используйте элемент [GroupingInformation](http://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) . 
    
2. С помощью параметров GroupingInformation и ExternalEwsUrl из откликов автообнаружения, почтовые ящики месте с GroupingInformation и ExternalEwsUrl объединяется значение в той же группе. Если всех групп, имеющих более чем 200 почтовые ящики, разбить групп дальнейший, чтобы каждая группа содержит не более 200 почтовых ящиков.
    
3. Создайте и используйте один объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) для остальной части процедуры. При использовании одного объекта **ExchangeService** , файлы cookie и заголовки (если они заданы), автоматически сохраняются. Обратите внимание на то, что если не требуется группа потоковой передачи подписок в одно, не для создания другого объекта **ExchangeService** для каждого пользователя с олицетворенным. 
    
4. [Отправить подписки](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) запрос для пользователей, имена которых сначала отображается, когда всем пользователям в группе сортируются в алфавитном порядке (мы будем называть этого пользователя в качестве пользователя почтового ящика привязки). Выполните следующие действия: 
    
  - Включите заголовок X-AnchorMailbox со значением, равным SMTP-адрес пользователя почтового ящика привязки.
    
  - Включите заголовок X-PreferServerAffinity со значением, равным true.
    
  - Используйте роль [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (тип [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
5. В ответе подписки получает значение X-BackEndOverrideCookie. Включите это значение в каждой из подписки на последующие запросы для пользователей в эту группу.
    
6. Для каждого дополнительного пользователя в группе отправить запрос подписки и сделайте следующее:
    
  - Включите заголовок X-AnchorMailbox со значением, равным SMTP-адрес пользователя почтового ящика привязки для группы.
    
  - Включите заголовок X-PreferServerAffinity со значением, равным true.
    
  - Включите X-BackEndOverrideCookie, который был возвращен в ответ подписки привязки почтового ящика пользователя.
    
  - Используйте роль [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) (тип [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
    Обратите внимание на то, сервер использует значения X-PreferServerAffinity и X BackendOverrideCookie друг с другом для выполнения маршрутизации на сервер почтовых ящиков. Заголовок X-AnchorMailbox также является обязательным, но обрабатывается на сервере, если два значения являются допустимыми. Если X-AnchorMailbox и X PreferServerAffinity — в запросе и X BackendOverrideCookie не указан, чтобы перенаправлять запросы используется значение X-AnchorMailbox.
    
    Так как X PreferServerAffinity и значения X BackendOverrideCookie выполнения маршрутизации, если когда-либо перемещение почтовых ящиков привязки к другой группе или сервера, логику не изменяется, поскольку X-BackendOverrideCookie будет перенаправлять запрос к правильному серверу для группы.
    
7. Отправка одного [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) запросов для группы и сделайте следующее: 
    
  - Включить [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) значений, возвращенных в каждой из них ответов для почтовых ящиков в группе. 
    
  - При наличии более чем 200 подписок для группы, создание нескольких запросов. Максимальное количество значений [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) необходимо включить в запрос равно 200. 
    
  - Если вам требуется несколько подключений, чем доступно для целевого почтового ящика, используйте учетную запись службы для олицетворения почтового ящика привязки группы; в противном случае не используйте олицетворения. В идеальном варианте необходимо олицетворить уникальный почтовых ящиков на [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [GetEvents](http://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) запрос, чтобы никогда не возникнет ограничения полосы пропускания. 
    
  - Используйте ApplicationImpersonation, если вам требуется [несколько подключений, чем доступно для целевого почтового ящика](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); в противном случае не используйте ApplicationImpersonation.
    
  - Включать заголовок X-PreferServerAffinity и присвойте ей значение true. Это значение автоматически включается, если вы используете объект **ExchangeService** , созданный на шаге 2. 
    
  - Включите BackEndOverrideCookie X для группы (X-BackEndOverrideCookie, который был возвращен в ответ подписки пользователя почтового ящика привязки). Это значение автоматически включается, если вы используете объект **ExchangeService** , созданный на шаге 2. 
    
8. Передайте возвращенные события отдельный поток для обработки.
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>Какие регулирования значения необходимо принять во внимание?
<a name="bk_throttling"> </a>

При планировании внедрения уведомлений, необходимо учитывать два значения: число подключений и число подписок. В следующей таблице перечислены значения по умолчанию для каждого из параметров [регулирования](ews-throttling-in-exchange.md) и как используются параметры. Для каждого значения бюджета, выделяемого для целевого почтового ящика. По этой причине использование олицетворения для получения дополнительных подключений шаг является обязательным в различных сценариях. 
  
**В таблице 1. Регулирования значения по умолчанию**

|**Область внимание**|**Параметр регулирования**|**Default value**|**Описание**|
|:-----|:-----|:-----|:-----|
|Потоковая передача подключений  <br/> |По умолчанию, выступающие ограничения подключения  <br/> |10 для Exchange Online  <br/> 3 для Exchange 2013  <br/> |Максимальное число одновременных подключений потоковой передачи, которые могут иметь учетную запись, одновременно открытых на сервере. Для работы в рамках это ограничение, использование учетной записи службы с помощью роль ApplicationImpersonation, назначенных для почтовых ящиков конечного и олицетворения первым пользователем в каждой группе идентификатор подписки при начало в потоке событий.  <br/> |
|Включения или отключения подключений  <br/> |EWSMaxConcurrency  <br/> |27  <br/> |Максимальное число одновременных подключений включения или отключения (запросов, которые получены, но еще не ответил), что локальная учетная запись может иметь open на сервере за один раз.  <br/> |
|Подписки  <br/> |EWSMaxSubscriptions  <br/> |20 для Exchange Online  <br/> 5000 для Exchange 2013  <br/> |Максимальное число nonexpired подписок учетной записи, у которых есть за один раз. Это значение уменьшается при создании подписки на сервере.  <br/> |
   
В следующем примере показано обработки бюджеты между любого целевого почтового ящика и учетной записи службы, имеющей роль [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) , назначенных для почтовых ящиков целевой. 
  
- ServiceAccount1 (sa1) олицетворяет число пользователей (m1, m2, m3 и т. д.) и создает подписки для каждого почтового ящика. Обратите внимание, что при создании подписок, владелец подписки sa1, поэтому при sa1 открывает подключение с подписок, веб-служб Exchange обеспечивает, что подписок принадлежат sa1.
    
- Sa1 можно открыть подключение следующими способами:
    
1. Без олицетворения поэтому подключение является вычитается sa1.
    
2. С помощью любого пользователя олицетворения — m1 для примера —, чтобы подключение, вычитается копию m1 бюджета. (M1 самого можно открывать подключений с помощью Exchange Online и все учетные записи служб, олицетворения m1 может подключений с помощью скопированного бюджета.)
    
- Если предела подключения доступны следующие решения:
    
  - Если используется параметр 1, администратор может создать несколько учетных записей служб для олицетворения дополнительных пользователей.
    
  - Если используется параметр 2, код может олицетворять другого пользователя — m2 для примера.
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>Пример: Обслуживание сходства между группой подписок и сервера почтовых ящиков
<a name="bk_ce"> </a>

Хорошо, давайте посмотрим в действии. В следующем примере кода показано, как группы пользователей и использование заголовков X-AnchorMailbox и X PreferServerAffinity и X BackendOverrideCookie cookie на обслуживание сходства с сервера почтовых ящиков. Поскольку роль в материале сходства заголовков и файл cookie, в этом примере в центре внимания XML веб-служб Exchange запросы и ответы. Чтобы использовать управляемый API веб-служб Exchange для создания тело подписки запросы и ответы, обратитесь к разделу [потока уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) и [уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange по запросу](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). В этом разделе содержатся дополнительные действия, относящиеся к обслуживанию сходства и добавление заголовков в ваших запросов.
  
В этом примере имеется четыре пользователей: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com и sadie@contoso.com. На следующем рисунке показана GroupingInformation и ExternalEwsUrl [Параметры автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) для пользователей. 
  
**На рисунке 1. Параметры автообнаружения, используемые для групповых почтовых ящиков**

![Таблица, в которой показаны значения параметров GroupingInformation и ExternalEwsUrl для каждого из пользователей.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
С помощью параметров из откликов автообнаружения, почтовые ящики сгруппированные по составное значения параметров GroupingInformation и ExternalEwsUrl. В этом примере Алексей и Sadie имеют те же значения, поэтому они находятся в одной группе и Alisa и Ronnie совместно использовать те же значения, поэтому они находятся в другую группу.
  
**На рисунке 2. Создание группы почтовых ящиков**

![Таблица, в которой показано, как группы почтовых ящиков создаются с помощью параметров автообнаружения.](media/Exchange2013_NotificationAffinityGrouping.png)
  
В этом примере мы рассмотрим а группы. Мы будет использовать те же действия для группы B, но используйте другое значение X-AnchorMailbox для этой группы.
  
С помощью [ApplicationImpersonation](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx), создайте запрос подписки для почтового ящика привязки (alfred@contoso.com), с помощью заголовка X-AnchorMailbox, задайте значение свой адрес электронной почты и значение заголовка X-PreferServerAffinity значение true. Установка значений этих двух заголовка вызовет сервер для создания X BackEndOverrideCookie для ответа.
  
Если вы используете управляемый API веб-служб Exchange, используйте метод[Add](http://msdn.microsoft.com/EN-US/library/cy7xta5e) [HttpHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)для добавления двух верхних запрос на подписку, как показано. 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

Поэтому запрос подписки пользователя Алексей выглядит следующим образом.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>alfred@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>
```

Следующее сообщение XML — это ответ на запрос пользователя Алексей подписки, а также X-BackEndOverrideCookie. Отправьте этот файл cookie для всех последующих запросов для пользователей в эту группу. Обратите внимание на то, что ответ также содержит дополнительные файлы cookie, такие как exchangecookie файла cookie, используемый Exchange 2010. Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013 игнорировать exchangecookie, если он включен в подписки на последующие запросы.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

С помощью BackEndOverrideCookie X из ответа пользователя Алексей и заголовок X-AnchorMailbox для Sadie создается запрос подписки, другой член группы A. Sadie запрос подписки выглядит следующим образом.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@consoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@consoso.com </t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:Subscribe>
      <m:StreamingSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox" />
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
        </t:EventTypes>
      </m:StreamingSubscriptionRequest>
    </m:Subscribe>
  </soap:Body>
</soap:Envelope>

```

Ответа подписки на Sadie выглядит следующим образом. Обратите внимание на то, что она не включает X-BackEndOverrideCookie. Клиент не отвечает за кэширования этого значения для последующих запросов.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</m:SubscriptionId>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </m:SubscribeResponse>
  </s:Body>
</s:Envelope>
```

Использование значений [SubscriptionId](http://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) из ответов подписки, был создан запрос операции [GetStreamingEvents](http://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) для всех подписок в группе. Из-за меньше, чем 200 подписки в эту группу, они все отправляются в один запрос. Заголовок X-PreferServerAffinity задано значение true и X-BackEndOverrideCookie включен. 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com</t:SmtpAddress>
      </t:ConnectingSID>
    </t:ExchangeImpersonation>
  </soap:Header>
  <soap:Body>
    <m:GetStreamingEvents>
      <m:SubscriptionIds>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAB4EQOy2pfrQJfM3hzs/nZJIZssan6H0Ag=</t:SubscriptionId>
        <t:SubscriptionId>JgBjbzFwcjA2bWIyMjIubmFtcHJkMDYucHJvZC5vdXRsb29rLmNvbRAAAAAUeGk+7JFdSaFM8/NI/gQQpVdgZX6H0Ag=</t:SubscriptionId>
      </m:SubscriptionIds>
      <m:ConnectionTimeout>10</m:ConnectionTimeout>
    </m:GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

Возвращенный события затем передаются в отдельном потоке для обработки.
  
## <a name="how-has-affinity-changed"></a>Как изменилось сходства?
<a name="bk_howchanged"> </a>

В Exchange 2010, подписок, сохраняются на сервере клиентского доступа, как показано на рисунке 3. В версиях Exchange, более поздней, чем Exchange 2010 подписок, сохраняются на сервере почтовых ящиков, как показано на рисунке 4.
  
**На рисунке 3. Процесс за обеспечение соответствия в Exchange 2010**

![Иллюстрация, показывающая принцип поддержки таблицы активных подписок на сервере клиентского доступа в Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
**На рисунке 4. Процесс за обеспечение соответствия в Exchange Online и Exchange 2013**

![Иллюстрация, показывающая, как балансировщик нагрузки и сервер клиентского доступа перенаправляют запросы на сервер почтовых ящиков, на котором хранится таблица активных подписок Exchange Server и Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
В Exchange 2010, клиент знает только адрес балансировщика нагрузки и exchangecookie, возвращенные сервером гарантирует, что запрос перенаправляется в правом сервера клиентского доступа. Тем не менее в более поздних версий, балансировки нагрузки и роли сервера клиентского доступа и нужно перенаправлять запросы должным образом, прежде чем они станут на сервер почтовых ящиков. Чтобы сделать, что необходима дополнительная информация, вот почему появились новые заголовки и файл cookie. Статья [подписки на уведомления, события почтового ящика и веб-службах Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) объясняется, как подписки поддерживаются в Exchange 2013. 
  
Пользователь может заметить, что более поздней версии по-прежнему возвращается exchangecookie, использующего Exchange 2010. Нет вреда, в том числе этот файл cookie в запросах, но более поздние версии Exchange игнорировать его.
  
## <a name="see-also"></a>См. также

- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Поток уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [По запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
- [Изменения в управлении сходства для подписок на веб-служб Exchange...](http://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [Веб-служб Exchange регулирования в Exchange](ews-throttling-in-exchange.md)
    

