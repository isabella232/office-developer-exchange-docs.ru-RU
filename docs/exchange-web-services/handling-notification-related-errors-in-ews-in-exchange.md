---
title: Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Узнайте, как обрабатывать ошибки, связанные с уведомлений в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: cb0c16a74e68b5a16ef0f2011f65b22675950f58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760955"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange

Узнайте, как обрабатывать ошибки, связанные с уведомлений в приложениях, разработка с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Если приложение подписывается на данные и получает уведомления, может потребоваться обрабатывать ошибки, связанные с уведомлений. Может обрабатывать эти ошибки во время выполнения или при разработке приложения веб-служб Exchange.
  
**В таблице 1. Ошибки, связанные с уведомления и для их обработки**

|Ошибка|Происходит при попытке...|Обработать его с...|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |Откройте подключение для получения событий, когда достигнут предел подключения из учетной записи откройте потоковой передачи подключений. | <ul><li>Использование [олицетворения](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) для [открытия подключения](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Использование меньшего числа подключений для получения событий. Повысить число подписок для каждого подключения с [помощью сходства](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md) , [поместив не более 200 подписки идентификаторы в ту же группу](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain). Затем можно использовать то же подключение для получения событий для всей группы, сокращения числа необходимых подключений.</li><li>  При изменении значения HangingConnectionLimit в файле web.config для локальную систему Exchange, чтобы переопределить значение по умолчанию из трех подключений. Exchange Online имеет по умолчанию HangingConnectionLimit 10, которая не настраивается.</li></ul> |
|**ErrorExceededSubscriptionCount** |Создание слишком большого числа подписок. [EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) параметр для политики регулирования определяет максимальное число подписок, которое может создать учетную запись. | <ul><li>Использование [олицетворения](http://technet.microsoft.com/en-us/library/dd776119%28v=exchg.150%29.aspx) для [создания подписок](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling).</li><li>Уменьшение числа подписок.</li></ul> |
|**ErrorInvalidSubscriptionRequest** |Создание подписок для нескольких почтовых ящиков или несколько папок из одного запроса.  |Создание подписки для одной общей папки или одного почтового ящика в одном запросе.| 
|**ErrorInvalidWatermark** |Получение событий с помощью недопустимый водяного знака.| <ul><li>Проверка подписки с Идентификатором возвращаются в предыдущем ответе.</li><li>Проверка того, что отправке идентификатор подписки для правильного объекта **ExchangeService** .</li><li>[Создание новой подписки](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**ErrorMissedNotificationEvents** |Получение событий при пропущены некоторые предыдущих событий.   |Сравнение свойства расширенного папки, которые **PR_LOCAL_COMMIT_TIME_MAX** (0x670a) и **PR_DELETED_COUNT_TOTAL** (0x670b), чтобы определить, какие изменения были пропущены и [Создание новой подписки](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).  |
|**ErrorProxyRequestNotAllowed** |Подпишитесь на события для пользователя в пакетной запрос, почтовый ящик которого был перемещен на другой сайт.   |Повторное обнаружение ExternalEwsUrl или EwsPartnerUrl с помощью [службы автообнаружения](autodiscover-for-exchange.md) и создание новой подписки.  |
|**ErrorReadEventsFailed** |Получение событий из подписки, который не удается найти.  |Повторное обнаружение ExternalEwsUrl или EwsPartnerUrl с помощью [службы автообнаружения](autodiscover-for-exchange.md) и создание новой подписки.  |
|**ErrorServerBusy** | Превышать пределы [регулирования](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) . Необходимо учитывать следующие отношении регулирования.<ul><li>[EwsMaxSubscriptions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) предел регулирования определяет максимальное число push, запросу или потоковая передача подписки на уведомления, которые могут быть активны единовременно. Это значение подписок на почтовый ящик, не число подписок отдельной папки в подписке почтового ящика. Начиная с версии почтовых ящиков службы 14.16.0135 и 14.15.0057.000 почтового ящика, размещенного Exchange Online или Exchange Online в составе Office 365 может иметь до 20 подписок и конечного Exchange 2013 локального почтового ящика могут иметь до 5000 подписок.</li><li>[EwsMaxConcurrency](http://msdn.microsoft.com/en-us/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) предел регулирования определяет максимальное число активных запросов для подключений, не являющиеся потоковая передача и имеет значение по умолчанию 27.</li><li>Ограничение по умолчанию для открытых подключений потоковой передачи, равно 10.</li></ul> |<ul><li>[Учитывая последствия регулирования политики, связанные с уведомлений](ews-throttling-in-exchange.md#bk_ThrottlingNotifications) и ограничение числа активных подписок и активных подключений, чтобы приложение не применяется регулирование.</li><li>Использование меньшего числа подключений для получения событий. Повысить число подписок для каждого подключения, [поместив не более 200 подписки идентификаторы в ту же группу](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md). Затем можно использовать то же подключение для получения событий для всей группы, сокращения числа необходимых подключений.</li><li>При изменении значения HangingConnectionLimit в файле web.config, чтобы переопределить значение по умолчанию из десяти открытых подключений потоковой передачи.</li></ul>|
|**ErrorSubscriptionNotFound** |Получение событий для подписки, который не удается найти. Может срока действия подписки, процесс веб-служб Exchange был перезагружен или передано недопустимое подписки. | <ul><li>Проверка того, что вы используете же идентификатор подписки, который был возвращен в предыдущем ответе.</li><li>Проверка того, что отправке идентификатор подписки для правильного объекта **ExchangeService** .</li><li> [Создание новой подписки](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover).</li></ul> |
|**[ServiceLocalException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Добавьте подписку в новую папку, когда подключение подписки открыт в другую папку.  |Изменение ее, чтобы подписаться на всех папок в почтовом ящике, а не указанной папки.  |
|**[ServiceResponseException](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Получение событий для подписки, который не удается найти в хранилище Exchange.  | <ul><li>Проверка того, что вы используете же идентификатор подписки, который был возвращен в предыдущем ответе.</li><li>Проверка того, что отправке идентификатор подписки для правильного объекта **ExchangeService** .</li></ul> |
   
## <a name="recovering-from-lost-subscriptions"></a>Восстановление после потеряны подписки
<a name="bk_recover"> </a>

При подписке теряются или больше не доступен, лучше создать новую подписку и не включать старые водяного знака в новой подписки. Resubscribing со старой водяного знака вызывает линейная сканирования для событий, который обходится дорого. Вместо этого создайте новую подписку и сравнение свойства папки для поиска изменений в содержимое, которое произошло между потеряны подписки и создать подписку. Свойства расширенной папки, которые рекомендуется проверять, **PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040) и **PR_DELETED_COUNT_TOTAL** (0x670b0003). Это можно сделать, [Создание определения расширенных свойств](properties-and-extended-properties-in-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также

- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Поток уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [По запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)    
- [Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    

