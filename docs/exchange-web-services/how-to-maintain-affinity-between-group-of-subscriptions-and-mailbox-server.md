---
title: Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 1bda4094-88c3-4f61-9219-6ee70f6e81cf
description: Сведения о поддержке сходства между группой подписок и сервером почтовых ящиков.
localization_priority: Priority
ms.openlocfilehash: 1618216cf69e08b2ae774264e0910856a59851af
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455772"
---
# <a name="maintain-affinity-between-a-group-of-subscriptions-and-the-mailbox-server-in-exchange"></a>Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange

Сведения о поддержке сходства между группой подписок и сервером почтовых ящиков.
  
Сходство это ассоциация последовательности запросов и ответных сообщений с определенным сервером почтовых ящиков. Для большинства функциональных возможностей Exchange сервер обрабатывает сходство. Однако уведомления являются исключением. Клиент отвечает за поддержание сходства с сервером почтовых ящиков для подписок на уведомления. Это сходство позволяет серверам подсистемы балансировки нагрузки и клиентского доступа между клиентом и сервером маршрутизировать подписки на уведомления и связанные запросы на сервер почтовых ящиков, который обслуживает подписку. Без сходства запрос может направляться на другой сервер почтовых ящиков, который не включает подписки клиента, что может привести к возвращению ошибки [еррорсубскриптионнотфаунд](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) . 
  
## <a name="how-is-affinity-maintained"></a>Как поддерживается сходство?
<a name="bk_howmaintained"> </a>

Сходство в Exchange — на основе файлов cookie. Клиент запускает создание файла cookie, включая определенные заголовки в запросе на подписку, а затем ответ на подписку содержит файл cookie. Затем клиент отправляет этот файл cookie в последующих запросах, чтобы убедиться, что запрос перенаправляется на подходящий сервер почтовых ящиков.
  
Точнее, сходство в Exchange обрабатывается следующим образом: 
  
- X-AnchorMailbox — HTTP-заголовок, включенный в начальный запрос на подписку. Он определяет первый почтовый ящик в группе почтовых ящиков, которые совместно используют сходство с одним и тем же сервером почтовых ящиков.
    
- X-Преферсервераффинити — HTTP-заголовок, который включается в начальный запрос подписки с помощью заголовка X-AnchorMailbox и имеет значение true, чтобы указать, что клиент запрашивает сопоставление соответствия с сервером почтовых ящиков.
    
- X-Баккендоверридекукие — файл cookie, который включен в первоначальный ответ подписки и содержит файл cookie, используемый сервером балансировки нагрузки и сервером клиентского доступа для маршрутизации последующих запросов на один сервер почтовых ящиков.
    
## <a name="how-do-i-maintain-affinity-by-using-the-ews-managed-api-or-ews"></a>Как сохранить сходство с помощью управляемого API EWS или EWS?
<a name="bk_howdoimaintain"> </a>

Вы можете использовать одни и те же действия для сохранения сходства для нескольких подписок почтовых ящиков и их серверов почтовых ящиков независимо от того, используете ли вы уведомления о потоках, опрашивающей или Push-связи, независимо от того, используете ли вы локальный сервер Exchange или Exchange Online.
  
1. Для каждого почтового ящика [вызовите службу автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и получите параметры Граупингинформатион и екстерналевсурл пользователя. Для автообнаружения SOAP вы используете элемент [Setting](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) , а для службы автообнаружения POX — элемент [граупингинформатион](https://msdn.microsoft.com/library/2d8a007f-d79c-43c8-90e3-2c6d883f3a7c%28Office.15%29.aspx) . 
    
2. С помощью параметров Граупингинформатион и Екстерналевсурл из откликов автообнаружения помещайте почтовые ящики с одинаковым значением Екстерналевсурл и Граупингинформатион сцепления в одну группу. Если в одной из групп больше 200 почтовых ящиков, разделите их, чтобы в каждой группе было не более 200 почтовых ящиков.
    
3. Создайте и используйте один объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=EXCHG.80%29.aspx) для оставшейся части процедуры. При использовании одного и того же объекта **ExchangeService** файлы cookie и заголовки (при их задании) автоматически сохраняются. Обратите внимание, что если вы не планируете группировать почтовые подписки в единое подключение, вы можете создать отдельный объект **ExchangeService** для каждого олицетворенного пользователя. 
    
4. [Отправьте запрос на подписку](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) для пользователя, имя которого отображается в алфавитном порядке, когда все пользователи в группе сортируются в алфавитном порядке (этот пользователь будет называться пользователь почтовых ящиков привязки). Выполните указанные ниже действия. 
    
  - Включите заголовок X-AnchorMailbox со значением, равным SMTP-адресу пользователя закрепленного почтового ящика.
    
  - Включите заголовок X – Преферсервераффинити со значением true.
    
  - Используйте роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (тип [ексчанжеимперсонатион](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
5. В ответе на подписку получите значение X – Баккендоверридекукие. Включите это значение в каждую из последующих запросов подписки для пользователей в этой группе.
    
6. Для каждого дополнительного пользователя в группе отправьте запрос на подписку и выполните следующие действия:
    
  - Включите заголовок X-AnchorMailbox со значением, равным SMTP-адресу пользователя закрепленного почтового ящика пользователя для группы.
    
  - Включите заголовок X – Преферсервераффинити со значением true.
    
  - Включите X – Баккендоверридекукие, возвращенный в ответе на подписку пользователя привязанного почтового ящика.
    
  - Используйте роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) (тип [ексчанжеимперсонатион](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) ). 
    
    Обратите внимание, что сервер использует значения X – Преферсервераффинити и X Баккендоверридекукие для выполнения маршрутизации на сервер почтовых ящиков. Заголовок X-AnchorMailbox также необходим, но он игнорируется сервером, если остальные два значения являются допустимыми. Если X-AnchorMailbox и X-Преферсервераффинити находятся в запросе, а X-Баккендоверридекукие не включено, то для маршрутизации запросов используется значение X-AnchorMailbox.
    
    Так как значения X-Преферсервераффинити и X-Баккендоверридекукие выполняют маршрутизацию, если почтовый ящик привязки когда-либо перемещается в другую группу или на другой сервер, то логика не изменяется, так как X-Баккендоверридекукие направляет запрос на правильный сервер для группы.
    
7. Отправьте отдельные запросы [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [Events](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) для группы и выполните следующие действия: 
    
  - Включите значения [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) , возвращенные в каждом из ответов на отдельные подписки для почтовых ящиков в группе. 
    
  - Если для группы существует более 200 подписок, создайте несколько запросов. Максимальное число значений [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) , включаемых в запрос: 200. 
    
  - Если требуется больше подключений, чем доступно для целевого почтового ящика, используйте учетную запись службы для олицетворения почтового ящика привязки для группы; в противном случае не используйте олицетворение. В идеале необходимо олицетворять уникальный почтовый ящик на запрос [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) или [Events](https://msdn.microsoft.com/library/22d4da6b-d8a8-484f-82c4-3e4b8f5431cd%28Office.15%29.aspx) , чтобы никогда не применялись ограничения на регулирование. 
    
  - Используйте ApplicationImpersonation, если вам требуется [больше подключений, чем доступно для целевого почтового ящика](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling); в противном случае не используйте ApplicationImpersonation.
    
  - Включите заголовок X – Преферсервераффинити и задайте для него значение true. Это значение автоматически включается при использовании объекта **ExchangeService** , созданного на шаге 2. 
    
  - Включите X-Баккендоверридекукие для группы (X-Баккендоверридекукие, которая была возвращена в ответе на подписку пользователя привязанного почтового ящика). Это значение автоматически включается при использовании объекта **ExchangeService** , созданного на шаге 2. 
    
8. Передайте возвращенные события в отдельный поток для обработки.
    
## <a name="what-throttling-values-do-i-need-to-take-into-consideration"></a>Какие значения регулирования необходимо учитывать?
<a name="bk_throttling"> </a>

При планировании реализации уведомлений необходимо учитывать два значения: количество подключений и число подписок. В следующей таблице приведены значения по умолчанию для каждого параметра [регулирования](ews-throttling-in-exchange.md) и способов использования этих параметров. Для каждого значения бюджет размещается в целевом почтовом ящике. По этой причине использование олицетворения для получения дополнительных подключений является обязательным шагом во многих сценариях. 
  
**Таблица 1. Значения регулирования по умолчанию**

|**Область рассмотрения**|**Параметр регулирования**|**Значение по умолчанию**|**Описание**|
|:-----|:-----|:-----|:-----|
|Потоковое подключение  <br/> |Предельное число подключений по умолчанию  <br/> |10 для Exchange Online  <br/> 3 для Exchange 2013  <br/> |Максимальное число одновременных потоков подключений, которые могут быть открыты учетной записью на сервере в один момент времени. Для работы с этим пределом используйте учетную запись службы с ролью ApplicationImpersonation, назначенной для целевых почтовых ящиков, и олицетворяет первого пользователя в каждой группе ИДЕНТИФИКАТОРов подписки, когда вы получаете потоковые события.  <br/> |
|Опрашивающие или Push-подключения  <br/> |евсмаксконкурренци  <br/> |27  <br/> |Максимальное количество одновременных запросов на получение или принудительной передачи (запросов, которые еще не ответили), которые учетная запись может открыть на сервере в один момент времени.  <br/> |
|Подписки  <br/> |евсмакссубскриптионс  <br/> |20 для Exchange Online  <br/> 5000 для Exchange 2013  <br/> |Максимальное число подписок с неистекшим сроком действия, которые могут одновременно находиться в учетной записи. Это значение уменьшается при создании подписки на сервере.  <br/> |
   
В приведенном ниже примере показано, как будут обрабатываться бюджеты между любым целевым почтовым ящиком и учетной записью службы, которой назначена роль [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) для целевых почтовых ящиков. 
  
- ServiceAccount1 (SA1) олицетворяет многих пользователей (M1, m2, M3 и т. д.) и создает подписки для каждого почтового ящика. Обратите внимание на то, что при создании подписок владелец подписки — SA1, поэтому когда SA1 открывает подключение с подписками, EWS применяет к ним владельца SA1.
    
- SA1 может открыть подключение следующими способами:
    
1. Без олицетворения, поэтому соединение будет взиматься с SA1.
    
2. Выполнив олицетворение любого пользователя (например, M1), чтобы подключение было взимать копию бюджета m1's. (M1 может открыть десять подключений с помощью Exchange Online, а все учетные записи служб, вызывающие M1, могут открыть десять подключений с помощью скопированного бюджета.)
    
- Если достигнуто максимальное число подключений, доступны следующие обходные пути:
    
  - Если используется вариант 1, администратор может создать несколько учетных записей служб для олицетворения дополнительных пользователей.
    
  - Если используется вариант 2, код может олицетворять другого пользователя — m2 для примера.
    
## <a name="example-maintaining-affinity-between-a-group-of-subscriptions-and-the-mailbox-server"></a>Пример: поддержание сходства между группой подписок и сервером почтовых ящиков
<a name="bk_ce"> </a>

Итак, давайте посмотрим, как это выполняется в действии. В приведенном ниже примере кода показано, как группировать пользователей и использовать заголовки X AnchorMailbox и X Преферсервераффинити, а также файл cookie X – Баккендоверридекукие для поддержки сходства с сервером почтовых ящиков. Так как заголовки и файлы cookie являются основным уровнем важности в цепочке сходства, в этом примере основное внимание уделяется запросам и ответам XML EWS. Чтобы использовать управляемый API EWS для создания основного текста запросов и ответов на подписку, обратитесь к разделу [Отправка уведомлений о событиях почтовых ящиков с помощью EWS в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md) и [уведомления о событиях почтовых ящиков с помощью EWS в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). В этом разделе приводятся дополнительные действия для поддержки сходства и добавления заголовков в запросы.
  
В этом примере имеются четыре пользователя: alfred@contoso.com, alisa@contoso.com, ronnie@contoso.com и sadie@contoso.com. На следующем рисунке показаны [Параметры автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) Граупингинформатион и екстерналевсурл для пользователей. 
  
**Рис. 1. Параметры автообнаружения, используемые для групповых почтовых ящиков**

![Таблица, в которой показаны значения параметров GroupingInformation и ExternalEwsUrl для каждого из пользователей.](media/Exchange2013_NotificationAffinityAutoDResults.png)
  
При использовании параметров из ответов автообнаружения почтовые ящики группируются по Объединенному значению параметров Граупингинформатион и Екстерналевсурл. В этом примере Алфред и Ольга имеют одинаковые значения, поэтому они находятся в одной группе, а Алиса и ронние имеют одни и те же значения, поэтому они находятся в другой группе.
  
**Рис. 2. Создание групп почтовых ящиков**

![Таблица, в которой показано, как группы почтовых ящиков создаются с помощью параметров автообнаружения.](media/Exchange2013_NotificationAffinityGrouping.png)
  
В этом примере основное внимание уделяется группе A. Мы будем использовать одни и те же действия для группы B, но использовать другое значение X-AnchorMailbox для этой группы.
  
С помощью [ApplicationImpersonation](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx)создайте запрос на подписку для почтового ящика привязки (Alfred@contoso.com), для которого в заголовке x-AnchorMailbox задан адрес электронной почты, а для заголовка x-преферсервераффинити — значение true. Установка этих двух значений заголовков приведет к запуску сервера для создания Баккендоверридекукие X для ответа.
  
Если вы используете управляемый API EWS, используйте метод [хттфеадерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice_members%28v=exchg.80%29.aspx)[Add](https://msdn.microsoft.com/library/cy7xta5e) , чтобы добавить два заголовка в запрос на подписку, как показано ниже. 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", Mailbox.SMTPAddress);
service.HttpHeaders.Add("X-PreferServerAffinity", "true");
```

Поэтому запрос на подписку Алфред выглядит следующим образом.
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0516.014
X-AnchorMailbox: alfred@contoso.com
X-PreferServerAffinity: true
Host: outlook.office365.com
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Следующее XML-сообщение является ответом на запрос подписки Алфред и включает X-Баккендоверридекукие. Повторно отправить этот файл cookie для всех последующих запросов пользователей в этой группе. Обратите внимание, что в ответе также содержатся дополнительные файлы cookie, например файл cookie ексчанжекукие, используемый Exchange 2010. Exchange Online, Exchange Online в составе Office 365 и версии Exchange, начиная с Exchange 2013, игнорируйте ексчанжекукие, если он включен в последующие запросы подписки.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=ddb8c383aef34c7694132aa679744feb; expires=Thu, 25-Sep-2014 18:42:45 GMT; path=/;
    HttpOnly
Set-Cookie: X-BackEndOverrideCookie=CO1PR06MB222.namprd06.prod.outlook.com~1941996295; path=/; secure; HttpOnly
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
    expires=Wed, 25-Sep-2013 18:52:49 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

При использовании ответа X-Баккендоверридекукие из отклика Алфред и заголовка X-AnchorMailbox запрос на подписку создается для Ольга, а другой участник группы A. Ольга-запроса на подписку выглядит следующим образом.
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
    <t:ExchangeImpersonation>
      <t:ConnectingSID>
        <t:SmtpAddress>sadie@contoso.com </t:SmtpAddress>
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

Ответ на подписку Ольга выглядит следующим образом. Обратите внимание, что он не включает X – Баккендоверридекукие. Клиент отвечает за кэширование этого значения для будущих запросов.
  
```XML
HTTP/1.1 200 OK
Content-Type: text/xml; charset=utf-8
Set-Cookie: exchangecookie=640ea858f69d47ff8cce8b44c337f6d9; path=/
Set-Cookie: X-BackEndCookie=alfred@contoso.com=Ox8XKzcXLxg==; 
   expires= Wed, 25-Sep-2013 18:53:06 GMT; path=/EWS; secure; HttpOnly
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="775"
                         MinorBuildNumber="7"
                         Version="V2_4"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

С помощью значений [SubscriptionId](https://msdn.microsoft.com/library/3f86c178-2311-4844-82db-c2a0e469d116%28Office.15%29.aspx) из ответов на подписку был создан запрос [GetStreamingEvents](https://msdn.microsoft.com/library/dbe83857-c4f8-4d98-813f-e03c289697a1%28Office.15%29.aspx) для всех подписок в группе. Так как в этой группе менее 200 подписок, все они отправляются в одном запросе. Для заголовка X-Преферсервераффинити задано значение true, а также включен параметр X-Баккендоверридекукие. 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Возвращаемые события затем передаются в отдельный поток для обработки.
  
## <a name="how-has-affinity-changed"></a>Как изменилось сходство?
<a name="bk_howchanged"> </a>

В Exchange 2010 подписки хранятся на сервере клиентского доступа, как показано на рисунке 3. В более поздних версиях Exchange, чем Exchange 2010, подписки хранятся на сервере почтовых ящиков, как показано на рисунке 4.
  
**Рис. 3. Процесс поддержания сходства в Exchange 2010**

![Иллюстрация, показывающая принцип поддержки таблицы активных подписок на сервере клиентского доступа в Exchange 2010.](media/Exchange2013_NoficationAffinity2010.png)
  
**На рисунке 4. Процесс поддержания сходства в Exchange Online и Exchange 2013**

![Иллюстрация, показывающая, как балансировщик нагрузки и сервер клиентского доступа перенаправляют запросы на сервер почтовых ящиков, на котором хранится таблица активных подписок Exchange Server и Exchange Online.](media/Exchange2013_NoficationAffinity2013.png)
  
В Exchange 2010 клиент знает только адрес подсистемы балансировки нагрузки, а ексчанжекукие, возвращенный сервером, гарантирует, что запрос перенаправляется на подходящий сервер клиентского доступа. Однако в более поздних версиях подсистема балансировки нагрузки и роли сервера клиентского доступа должны правильно маршрутизировать запросы, прежде чем они будут переданы на сервер почтовых ящиков. Для этого требуются дополнительные сведения, поэтому были введены новые заголовки и файлы cookie. Подписки на [уведомления, события почтовых ящиков и EWS в Exchange в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) поясняют, как поддерживаются подписки в Exchange 2013. 
  
Вы можете заметить, что ексчанжекукие, используемый Exchange 2010, по-прежнему возвращается в более поздних версиях. Включение этого файла cookie в запросы не является вредом, но последующие версии Exchange игнорируют его.
  
## <a name="see-also"></a>См. также

- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
- [Изменения в управлении сходством для подписок EWS...](https://blogs.msdn.com/b/mstehle/archive/2013/04/17/changes-in-managing-affinity-for-ews-subscriptions.aspx)
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    

