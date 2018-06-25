---
title: Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 76136f28-0dad-4ecc-9dd7-a45a1861e4b0
description: Сведения о подписках на уведомления и событии почтовых ящиков в EWS в Exchange.
ms.openlocfilehash: 4f466c6cc01af410807948a9fec40c2af399c3e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761239"
---
# <a name="notification-subscriptions-mailbox-events-and-ews-in-exchange"></a>Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о подписках на уведомления и событии почтовых ящиков в EWS в Exchange.
  
Чтобы подписаться на уведомления о событиях, возникающих в почтовом ящике или в одной или нескольких папках почтового ящика, можно использовать управляемый API EWS или веб-службы Exchange (EWS). Доступно три типа подписки: на потоковые уведомления, на уведомления по запросу и на push-уведомления. Каждый тип подписки использует собственные методы для получения уведомлений.
  
## <a name="getting-notifications---what-are-my-options"></a>Какие уведомления выбрать?
<a name="bk_notiftypes"> </a>

Службы EWS предлагают три типа подписки, которые независимо друг от друга уведомляют клиента об изменениях на сервере. Не имеет значения, какую именно подписку вы выберете, вы получите те же самые события уведомлений, отличаться будет только способ получения.
  
**Таблица 1. Типы подписки**

|**Возможные варианты**|**Описание**|**Насколько мне это подходит?**|
|:-----|:-----|:-----|
|Потоковые уведомления  <br/> |Уведомления, которые сервер отправляет через соединение, открытое в течение определенного периода времени.  <br/> |Потоковые уведомления рекомендуются для большинства приложений. Они похожи на уведомления по запросу и push-уведомления и объединяют в себе свойства обоих указанных типов. После создания подписки на уведомления соединение остается открытым до 30 минут, чтобы сервер успел передать уведомления клиенту. В данном случае не требуется запрашивать обновления, как при подписке на уведомления по запросу. Кроме того, не требуется создавать приложение прослушивателя для веб-службы, которое необходимо для получения push-уведомлений.  <br/> |
|Уведомления по запросу  <br/> |Уведомления, запрашиваемые или извлекаемые клиентом.  <br/> |Уведомления по запросу больше подходят для слабо связанных клиентов, где клиент ненадежно подключен к сети. Эти уведомления могут создавать дополнительный трафик между клиентом и сервером, так как клиент отправляет частые запросы к серверу для получения уведомлений, не все из которых приносят результат.  <br/> |
|Push-уведомления  <br/> |Уведомления, отправляемые (или принудительно отправляемые) сервером в веб-службу на стороне клиента через адрес обратного вызова.  <br/> |Как правило, push-уведомления приходят быстрее, чем уведомления по запросу. Кроме того, они подходят для сильно связанных клиентов с IP-адресом, к которым у сервера есть надежный доступ. Тем не менее push-уведомления стали реже использовать после появления потоковых уведомлений в Exchange 2010. Мы также рекомендуем использовать потоковые уведомления вместо push-уведомлений, если это возможно. Кроме того, для использования push-уведомлений требуется написать приложение прослушивателя, в котором и происходит принудительная отправка уведомлений. Уменьшение сетевого трафика  это основное, хоть и незначительное, преимущество данного типа уведомлений по сравнению с уведомлениями по запросу, которое, тем не менее, сводится на нет необходимостью создания отдельного приложения.  <br/> |
   
## <a name="what-ews-events-can-i-subscribe-to"></a>На какие события служб EWS можно подписаться?
<a name="bk_eventtypes"> </a>

Типы событий служб EWS, на которые возможна подписка, определены в статьях "[Перечисление EventType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx)" для управляемого API EWS или "Элемент [EventType](http://msdn.microsoft.com/library/04b70f9e-c226-4130-958e-0db0275cf58b%28Office.15%29.aspx)" для служб EWS. Подписка доступна для следующих событий службы EWS: 
  
- NewMail  в папку "Входящие" поступило новое сообщение.
    
- Deleted  сообщение безвозвратно удалено из папки "Входящие". Больше об уведомлениях для элементов можно узнать в статьях [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md) и [По запросу уведомления для событий, связанных с удаления почтового ящика веб-служб Exchange в Exchange](pull-notifications-for-ews-deletion-related-mailbox-events-in-exchange.md).
    
- Modified  изменился элемент или папка.
    
- Moved  элемент или папка перемещены. 
    
- Copied  скопирован элемент или папка.
    
- Created  создан элемент или папка. 
    
- FreeBusyChanged  изменились сведения о доступности пользователя.
    
Еще один тип событий служб EWS, событие Status, определяется элементом [EventType](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.eventtype%28v=exchg.80%29.aspx). На это событие не надо подписываться. Оно отправляется сервером для проверки состояния клиента (только для потоковых и push-уведомлений). Клиент должен ответить на это событие или он будет отключен по истечении времени ожидания. 
  
Одно действие пользователя может привести к созданию нескольких уведомлений. На рисунке ниже приводится ряд распространенных сценариев и уведомлений, созданных для каждого из них. На получение уведомлений влияют настройки клиента, поэтому приведенный список может быть дополнен другими вариантами конфигураций и соответствующими уведомлениями.
  
**Рисунок 1. Типы событий, возвращаемые подписками на уведомления**

![Таблица, в которой показаны уведомления, отправляемые пользователям в распространенных ситуациях, например при получении нового сообщения, создании новой папки, перемещении папок и т. д.](media/Exchange2013_Notifications_Events.png)
  
На рисунке 1 показан упрощенный процесс создания уведомления. На самом деле, для одного действия пользователя может быть создано несколько уведомлений (даже если они относятся к одному типу). Например, при переносе папки создается три события папки: одно для изменения папки, одно для бывшей родительской папки и еще одно для новой родительской папки. Так как для одной операции может быть создано несколько событий, мы рекомендуем [при создании операции синхронизации задать время ожидания в несколько секунд](mailbox-synchronization-and-ews-in-exchange.md#bk_bestpractices), чтобы синхронизация происходила только после завершения операции.
  
Кроме того, следует принимать во внимание, что параметры конфигурации, задаваемые конкретным пользователем, также влияют на создание уведомлений. Например, сведения о доступности некоторых пользователей обновляются автоматически, поэтому событие FreeBusyChanged создается в момент получения приглашения на собрание, которое пользователь часто еще не успел прочесть. Если же пользователи, не настраивали обновление сведений о доступности, событие FreeBusyChanged создается, только когда приглашение на собрание будет принято. Эти параметры могут оказывать значительное влияние на уведомления, создаваемые сервером.
  
## <a name="how-do-ews-notifications-work"></a>Принципы работы уведомлений служб EWS
<a name="bk_howwork"> </a>

Уведомления служб EWS обрабатываются на основании подписки. Обычно для одного почтового ящика создается одна подписка, которая позволяет подписаться на все папки или на некоторые из них. Решите на какие уведомления подписываться (потоковые уведомления, уведомления по запросу или push-уведомления), сведения о каких событиях получать (NewMail, Created, Deleted, Modified и т. д.), а затем создайте подписку. После этого сервер почтового ящика будет асинхронно отправлять клиенту события службы EWS. (Для справки: события синхронны в Exchange 2007, а в Exchange 2010 они хранятся на сервере клиентского доступа, но это не относится к более поздним версиям.)
  
Способы отправки уведомлений клиенту отличаются в зависимости от выбранного типа подписки. В этом разделе содержатся дополнительные сведения о принципах работы каждого из них.
  
### <a name="ews-streaming-notifications"></a>Потоковые уведомления служб EWS
<a name="bk_streamnotif"> </a>

Потоковые уведомления используют ожидающий запрос GET для сервера, чтобы соединение для подписки с потоковой передачей оставалось открытым. Таким образом, выполняется немедленная потоковая передача клиенту всех событий, происходящих, пока соединение активно. Во время одного подключения может быть отправлено несколько уведомлений. Соединение остается открытым в течение определенного времени, но не более 30 минут. После чего клиент снова отправляет ожидающий запрос GET. На рисунке 2 показан принцип работы подписок с потоковой передачей и потоковых уведомлений.
  
**Рисунок 2. Обзор потоковых уведомлений**

![Иллюстрация, показывающая принцип работы потоковых уведомлений. Чтобы настроить потоковые уведомления, сделайте следующее. 1. Оформите подписку. 2. Откройте соединение. 3. Дождитесь событий 4. Получите события, повторяйте шаги 3 и 4. 5. Закройте или оставьте соединение. 6. Отмените подписку или дождитесь, когда истечет срок ее действия.](media/Exchange2013_Notifications_StreamSub.png)
  
Сведения о создании потоковой передачи уведомлений видеть [потока уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md).
  
### <a name="ews-pull-notifications"></a>Уведомления по запросу служб EWS
<a name="bk_pullnotif"> </a>

Для получения уведомлений по запросу клиент запрашивает их через определенный, регулируемый им интервал. В результате могут приходить ответы GetEvents без уведомлений. На рисунке 3 показан принцип работы подписок и уведомлений по запросу.
  
**Рисунок 3. Обзор уведомлений по запросу**

![Иллюстрация, показывающая принцип работы pull-уведомлений. Чтобы настроить pull-уведомления, сделайте следующее. 1. Оформите подписку. 2. Отправьте события GetEvent. 3. Получив ответ, повторяйте пункты 2 и 3. 4. Закройте и оставьте соединение. 5. Отмените подписку или дождитесь, когда истечет срок ее действия.](media/Exchange2013_Notifications_PullSub.png)
  
Сведения о создании уведомлений опрашивающей [репликации по запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)см.
  
### <a name="ews-push-notifications"></a>Push-уведомления служб EWS
<a name="bk_pushnotif"> </a>

Сервер принудительно отправляет push-уведомления обратно клиенту, поэтому трафик используется только при передаче уведомления. На рисунке 4 показан принцип работы принудительных подписок и push-уведомлений.
  
**Рисунок 4. Обзор push-уведомлений**

![Иллюстрация, показывающая принцип работы push-уведомлений. Чтобы настроить push-уведомления, сделайте следующее. 1. Создайте слушателя, 2. Оформите подписку. 3. Дождитесь событий. 4. Получите события. 5. Отправьте ответ "ОК", повторите шаги 3, 4 и 5. 6. Отмените подписку или дождитесь, когда истечет срок ее действия.](media/Exchange2013_Notifications_PushSub.png)
  
Если вы используете [push-уведомления в Exchange 2010](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx), рекомендуем перейти к [использованию потоковых уведомлений](http://code.msdn.microsoft.com/exchange/Exchange-2013-Set-push-82738cc5) в приложении, в этом случае вам не понадобится отдельное приложение для получения событий.
  
## <a name="how-do-i-subscribe-to-notifications"></a>Как подписаться на уведомления?
<a name="bk_notifoperations"> </a>

Существует несколько вариантов подписки на уведомления в зависимости от типа подписки, который нужно создать.
  
**Таблица 2. Методы подписки на уведомления и необходимые операции**

|**Тип подписки**|**Операция служб EWS**|**Методы управляемого API EWS**|**Назначение**|
|:-----|:-----|:-----|:-----|
|Подписка с потоковой передачей  <br/> |[Операции подписки](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |Метод [ExchangeService.BeginSubscribeToStreamingNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> Метод [ExchangeService.BeginSubscribeToStreamingNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetostreamingnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> Метод [ExchangeService.SubscribeToStreamingNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetostreamingnotifications%28v=exchg.80%29.aspx) <br/> |Создает запрос подписки на потоковые уведомления.  <br/> |
|Подписка по запросу  <br/> |[Операции подписки](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |Метод [ExchangeService.BeginSubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotifications%28v=exchg.80%29.aspx) <br/> Метод [ExchangeService.BeginSubscribeToPullNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> Метод [ExchangeService.SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) <br/> Метод [ExchangeService.SubscribeToPullNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Создает запрос подписки на уведомления по запросу.  <br/> |
|Принудительная подписка  <br/> |[Операции подписки](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) <br/> |Перегруженный метод [ExchangeService.BeginSubscribeToPushNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotifications%28v=exchg.80%29.aspx) <br/> Перегруженный метод [ExchangeService.BeginSubscribeToPushNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.beginsubscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> Перегруженный метод [ExchangeService.SubscribeToPushNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx) <br/> Перегруженный метод [ExchangeService.SubscribeToPushNotificationsOnAllFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotificationsonallfolders%28v=exchg.80%29.aspx) <br/> |Создает запрос подписки на push-уведомления.  <br/> |
   
## <a name="how-do-i-get-ews-events"></a>Как получить события служб EWS?
<a name="bk_getevents"> </a>

Способ отправки данных о фактических событиях зависит от типа созданной вами подписки. 
  
Для потоковых уведомлений необходимо создать соединение для подписки с потоковой передачей, а затем добавить в него нужную подписку. Можно прочитать подробнее об этом процессе [потока уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
Для репликации по запросу уведомлений объект подписки инициализации при создании подписки, поэтому необходимо вызвать метод **GetEvent** или операции для получения событий на сервере. Можно получить дополнительные сведения в [по запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md). 
  
В таблице ниже перечислены операции и классы, необходимые для получения событий. 
  
**Таблица 3. Элементы и классы для создания соединения и получения событий**

|**Тип подписки**|**Операция служб EWS**|**Метод управляемого API EWS**|**Назначение**|
|:-----|:-----|:-----|:-----|
|Подписка с потоковой передачей  <br/> |[Операция GetStreamingEvents](http://msdn.microsoft.com/library/8da95423-72bc-4034-90a8-162eedcd059b%28Office.15%29.aspx) <br/> |Метод [StreamingSubscriptionConnection.AddSubscription](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.addsubscription%28v=exchg.80%29.aspx) <br/> |Создает на сервере ожидающий запрос GET, ответ на который приходит при возникновении какого-либо события.  <br/> |
|Подписка по запросу  <br/> |[Операция GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) <br/> |Метод [PullSubscription.GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) <br/> |Получает с сервера уведомления по запросу.  <br/> |
|Принудительная подписка  <br/> |Не применимо.  <br/> |Не применимо.  <br/> |Push-уведомления автоматически отправляются на прослушиватель для веб-службы (URL-адрес обратного вызова указывается в запросе на подписку). Не требуется вызывать дополнительные методы или операции.  <br/> |
   
## <a name="how-do-i-unsubscribe-to-notifications"></a>Как отменить подписку на уведомления?
<a name="bk_notifunsubscribe"> </a>

В таблице ниже указаны способы отмены подписки на различные типы уведомлений.
  
**Таблица 4. Методы отмены подписки на уведомления и необходимые операции**

|**Тип подписки**|**Службы EWS**|**Управляемый API EWS**||
|:-----|:-----|:-----|:-----|
|Подписка с потоковой передачей  <br/> |[Операция по отмене подписки](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |Метод [StreamingSubscription.BeginUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> Метод [StreamingSubscription.EndUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> Метод [StreamingSubscription.Unsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Подписка по запросу  <br/> |[Операция по отмене подписки](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) <br/> |Метод [PullSubscription.BeginUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.beginunsubscribe%28v=exchg.80%29.aspx) <br/> Метод [PullSubscription.EndUnsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.endunsubscribe%28v=exchg.80%29.aspx) <br/> Метод [PullSubscription.Unsubscribe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.unsubscribe%28v=exchg.80%29.aspx) <br/> ||
|Принудительная подписка  <br/> |Верните значение **Unsubscribe** в элементе [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx) элемента [SendNotificationResponseMessage](http://msdn.microsoft.com/library/2c6d681b-67ac-4331-bc6b-a2e709b638e3%28Office.15%29.aspx) <br/> |Не применимо. Подождите, пока истечет время ожидания для подписки.  <br/> ||
   
Вы также можете дождаться окончания времени ожидания для любой из подписок. 
  
**Таблица 5. Окончание времени ожидания для подписок**

|**Тип подписки**|**Значение времени ожидания в службах EWS**|**Значение времени ожидания в управляемом API EWS**|**Обработка времени ожидания**|
|:-----|:-----|:-----|:-----|
|Подписка с потоковой передачей  <br/> |Элемент [ConnectionTimeout](http://msdn.microsoft.com/library/14da68a0-bcca-4281-a774-47644baa4ee9%28Office.15%29.aspx)  <br/> | Параметр  *lifetime*  конструктора [StreamingSubscriptionConnection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.streamingsubscriptionconnection%28v=exchg.80%29.aspx)  <br/> |Для управляемого API EWS по истечении заданного значения времени ожидания запускается событие [OnDisconnect](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.ondisconnect%28v=exchg.80%29.aspx). Если не вызван метод [StreamingSubscriptionConnection.Open](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection.open%28v=exchg.80%29.aspx) соединение прерывается.  <br/> Для служб EWS по истечении заданного значения времени ожидания сообщение [GetUserConfigurationResponse](http://msdn.microsoft.com/library/5e418c91-c836-4de0-a80d-f0dad0c684d7%28Office.15%29.aspx) возвращает для элемента [ConnectionStatus](http://msdn.microsoft.com/library/4300f9d6-8bf9-48c2-9f07-d80197864e17%28Office.15%29.aspx) значение "Закрыто".  <br/> |
|Подписка по запросу  <br/> |Элемент [Timeout](http://msdn.microsoft.com/library/c2e1ca5a-6667-4f6f-aac4-89de33bddc54%28Office.15%29.aspx)  <br/> | Параметр  *timeout*  метода [SubscribeToPullNotification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx)  <br/> |По истечении заданного значения времени ожидания сервер удаляет подписку.  <br/> |
|Принудительная подписка  <br/> |Элемент [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx)  <br/> | Параметр  *frequency*  метода [SubscribeToPushNotification](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopushnotifications%28v=exchg.80%29.aspx)  <br/> |Если сервер не получает ответ на push-уведомление или проверку состояния связи, он несколько раз пытается отправить уведомление, а затем прекращает отправку. Дополнительные сведения см. в статье [StatusFrequency](http://msdn.microsoft.com/library/917474e2-a426-4166-b825-53783a41dad4%28Office.15%29.aspx).  <br/> |
   
## <a name="can-i-limit-subscriptions"></a>Можно ли ограничить подписки?
<a name="bk_limitsubs"> </a>

В локальном развертывании можно ограничить количество подписок для каждого пользователя с помощью параметра регулирования количества запросов [EwsMaxSubscriptions](ews-throttling-in-exchange.md) политики регулирования. Эту политику можно применить как ко всем пользователям, так и выборочно к некоторым из них. Политику регулирования **EwsMaxSubscriptions** невозможно настроить для Exchange Online. 
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_limitsubs"> </a>

- [Поток уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [По запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
- [Справочник по веб-службам для Exchange](../web-service-reference/web-services-reference-for-exchange.md)
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
- [Пример приложения для push-уведомлений](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)
    

