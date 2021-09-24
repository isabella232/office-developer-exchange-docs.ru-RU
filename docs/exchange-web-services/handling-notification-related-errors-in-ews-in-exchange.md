---
title: Обработка ошибок, связанных с уведомлениями, в EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 519e1e52-5f1f-4f06-931e-8c20a586a563
description: Узнайте, как обрабатывать ошибки, связанные с уведомлениями, в приложениях, которые вы разрабатываете с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 7b49a57b7236318e08cb70ac2ac00edc4cf86363
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520215"
---
# <a name="handling-notification-related-errors-in-ews-in-exchange"></a>Обработка ошибок, связанных с уведомлениями, в EWS в Exchange

Узнайте, как обрабатывать ошибки, связанные с уведомлениями, в приложениях, которые вы разрабатываете с помощью управляемого API EWS или EWS в Exchange.

Если приложение подписывается на уведомления и получает их, возможно, вам придется обрабатывать ошибки, связанные с уведомлением. Вы можете обрабатывать эти ошибки во время работы или во время разработки приложения EWS.

**Таблица 1. Ошибки, связанные с уведомлением, и их обработка**

|Error|Возникает при попытке...|Обработать его...|
|:-----|:-----|:-----|
|**ErrorExceededConnectionCount** |Откройте подключение для получения событий, когда учетная запись достигла предела подключения к открытым потоковым подключениям. | <ul><li>Использование [обезличения](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) для [открытия подключений.](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)</li><li>Использование меньшего количество подключений для получения событий. Максимальное количество подписок в каждом подключении с помощью [сродства](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md) и размещения не более [200](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howdoimaintain)подписок в одной группе . Затем можно использовать одно и то же подключение для получения событий для всей группы, уменьшая количество необходимых подключений.</li><li>  Изменение значения HangingConnectionLimit в файле web.config для Exchange локального значения для переопределения значения по умолчанию трех открытых подключений. Exchange Online по умолчанию hangingConnectionLimit 10, который не настраивается.</li></ul> |
|**ErrorExceededSubscriptionCount** |Создайте слишком много подписок. Параметр регулирования политики [регулирования EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) определяет максимальное количество подписок, которые может создать учетная запись. | <ul><li>Использование [обезличения](https://technet.microsoft.com/library/dd776119%28v=exchg.150%29.aspx) для [создания подписок.](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_throttling)</li><li>Уменьшение количества подписок.</li></ul> |
|**ErrorInvalidSubscriptionRequest** |Создание подписки для нескольких почтовых ящиков или нескольких папок из одного запроса.  |Создание подписки для одной общедоступных папок или одного почтового ящика в одном запросе.|
|**ErrorInvalidWatermark** |Получите события с помощью недействительных водяных знаков.| <ul><li>Проверка ИД подписки, возвращенного в предыдущем ответе.</li><li>Обеспечение отправки подписного ИД для правильного объекта **ExchangeService.**</li><li>[Создание новой подписки.](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)</li></ul> |
|**ErrorMissedNotificationEvents** |Получите события, когда некоторые предыдущие события были пропущены.   |Сравнение свойств расширенной папки  PR_LOCAL_COMMIT_TIME_MAX (0x670a) и **PR_DELETED_COUNT_TOTAL** (0x670b) для определения пропущенных изменений и создания новой [подписки.](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)  |
|**ErrorProxyRequestNotAllowed** |Подпишитесь на события для пользователя с пакетным запросом, почтовый ящик которого переместился на другой сайт.   |Использование [автооткрытия](autodiscover-for-exchange.md) для занового использования externalEwsUrl или EwsPartnerUrl и создания новой подписки.  |
|**ErrorReadEventsFailed** |Получите события из подписки, которую невозможно найти.  |Использование [автооткрытия](autodiscover-for-exchange.md) для занового использования externalEwsUrl или EwsPartnerUrl и создания новой подписки.  |
|**ErrorServerBusy** | [Превышение ограничений регулирования.](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) Будьте в курсе следующих направлений регулирования:<ul><li>Ограничение [регулирования регулирования EwsMaxSubscriptions](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxsubscriptions%28v=exchg.150%29.aspx) определяет максимальное количество подписок push, pull или streaming notification, которые могут быть одновременно активными. Это значение подписки на почтовые ящики, а не количество отдельных папок в подписке на почтовый ящик. Начиная с версий почтовых ящиков службы 14.16.0135 и 14.15.0057.000 почтовый ящик, на который Exchange Online или Exchange Online в составе Office 365, может иметь до 20 подписок, а целевой почтовый ящик Exchange 2013 года может иметь до 5000 подписок.</li><li>Ограничение [регулирования EwsMaxConcurrency](https://msdn.microsoft.com/library/microsoft.exchange.data.directory.systemconfiguration.throttlingpolicy.ewsmaxconcurrency%28v=exchg.150%29.aspx) определяет максимальное количество активных запросов для нестриминговых подключений и имеет значение по умолчанию 27.</li><li>Ограничение по умолчанию для открытых потокового подключения — десять.</li></ul> |<ul><li>[С учетом](ews-throttling-in-exchange.md#throttling-considerations-for-ews-notification-applications) последствий политики регулирования, связанной с уведомлениями, и ограничения количества активных подписок и активных подключений, чтобы приложение не было отлажено.</li><li>Использование меньшего количество подключений для получения событий. Увеличь количество подписок в каждом соединении, разместив не более [200](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)подписных ИД в одной группе. Затем можно использовать одно и то же подключение для получения событий для всей группы, уменьшая количество необходимых подключений.</li><li>Изменение значения HangingConnectionLimit в файле web.config переопределение значения по умолчанию десяти открытых потокового подключения.</li></ul>|
|**ErrorSubscriptionNotFound** |Получите события для подписки, которую невозможно найти. Возможно, срок действия подписки истек, процесс EWS мог быть перезапущен или была передана недействительный подписка. | <ul><li>Проверка того, что вы используете тот же ИД подписки, который был возвращен в предыдущем ответе.</li><li>Обеспечение отправки подписного ИД для правильного объекта **ExchangeService.**</li><li> [Создание новой подписки.](handling-notification-related-errors-in-ews-in-exchange.md#bk_recover)</li></ul> |
|**[ServiceLocalException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Добавьте подписку в новую папку, пока подключение к подписке открыто в другой папке.  |Изменение подписки на подписку на все папки в почтовом ящике вместо определенной папки.  |
|**[ServiceResponseException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponseexception%28v=exchg.80%29.aspx)** |Получите события для подписки, которая не может быть расположена в Exchange магазине.  | <ul><li>Проверка того, что вы используете тот же ИД подписки, который был возвращен в предыдущем ответе.</li><li>Обеспечение отправки подписного ИД для правильного объекта **ExchangeService.**</li></ul> |

## <a name="recovering-from-lost-subscriptions"></a>Восстановление после потерянной подписки
<a name="bk_recover"> </a>

Если подписка потеряна или больше недоступна, лучше всего создать новую подписку и не включать старый водяной знак в новую подписку. Повторное сканирование со старым водяным знаком вызывает линейное сканирование событий, которое является дорогостоящим. Вместо этого создайте новую подписку и сравните свойства папок, чтобы найти изменения контента, произошедшие между потерянной подпиской и новой подпиской. Свойства расширенной папки, которые мы рекомендуем проверить, **PR_LOCAL_COMMIT_TIME_MAX** (0x670a0040) и **PR_DELETED_COUNT_TOTAL** (0x670b0003). Это можно сделать, [создав расширенное определение свойства.](properties-and-extended-properties-in-ews-in-exchange.md)

## <a name="see-also"></a>См. также

- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
- [Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
- [Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)


