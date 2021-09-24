---
title: Функции EWS в разных версиях продуктов Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 186c51dc-ec33-4a5d-b739-c9fcb1d4cdd3
description: EWS реализует новые функции в выпусках новых продуктов. Используйте сведения в этой статье, чтобы определить, включена ли в Exchange адресная версия, которая включает поддержку данных или функций, к которые вам необходим доступ.
ms.openlocfilehash: bccd0e84fc28f8a7366f0463e555cceec71aa181
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512284"
---
# <a name="ews-functionality-in-exchange-product-versions"></a>Функции EWS в разных версиях продуктов Exchange

EWS реализует новые функции в выпусках новых продуктов. Используйте сведения в этой статье, чтобы определить, включена ли в Exchange адресная версия, которая включает поддержку данных или функций, к которые вам необходим доступ. 
  
В следующей таблице перечислены версии Exchange EWS и основные функции, которые были представлены в каждой версии.
  
## <a name="ews-features-by-product-version"></a>Функции EWS по версии продукта

|**Версия продукта**|**Компоненты**|
|:-----|:-----|
|Office 365 и Exchange Online |Включает все функции в текущей версии Exchange в дополнение к новым функциям, которые добавляются для онлайн-клиентов.  |
|Exchange 2013 SP1 | Включает все функции, Exchange 2013 г. В 2013 Exchange 2013 г. были представлены следующие функции:<ul><li>Теперь получение чтения можно приостановить для обновлений и удалений.</li><li>Вы можете получить [модерировать сведения об утверждении](https://msdn.microsoft.com/library/43a89f71-8002-4cb0-b3c8-1c2b2597f227%28Office.15%29.aspx) транспорта.</li><li>Можно просмотреть ответы на голосование.</li><li>Метод [SetHoldOnMailboxes](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setholdonmailboxes%28v=exchg.80%29.aspx) и операция [SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) принимают все параметры в одном объекте.</li><li>Поиск по обнаружению электронных данных может указывать язык поисковых запросов и формат для диапазонов дат, определенный для конкретной культуры.</li><li>Теперь [объект StreamingSubscriptionConnection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscriptionconnection%28v=exchg.80%29.aspx) может получить доступ к объектам [StreamingSubscription.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.streamingsubscription%28v=exchg.80%29.aspx)</li><li>В беседах есть параметр, который указывает, содержатся ли сообщения электронной почты, защищенные IRM.</li><li>Участники собраний могут предложить новое время начала и окончания собраний и включить их в ответ на собрания.</li><li>Метод автообнаружения [SOAP GetUserSettings](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.getusersettings%28v=exchg.80%29.aspx) возвращает параметр [GroupingInformation,](https://msdn.microsoft.com/library/office/dn529149%28v=exchg.150%29.aspx) который используется для поддержания сродства для нескольких подписок событий почтовых ящиков.</li></ul> |
|Exchange 2013  | Включает все функции, Exchange 2010 SP2. В 2013 Exchange были представлены следующие функции:  <ul><li>  Архивация</li><li>Обнаружение электронных данных</li><li>Personas</li><li>Политики хранения</li><li>Единое хранилище контактов</li><li>Фотографии пользователя</li></ul> |
|Exchange 2010 с пакетом обновления 2 (SP2)  | Включает в себя все функции, Exchange 2010 SP1. В 2010 Exchange 2010 г. были представлены следующие функции:  <ul><li>  Срок действия пароля</li><li>Точность DateTime</li><li>Обновленные идентификаторы свойств для контактов</li><li>Новые сценарии обезличения</li></ul> |
|Exchange 2010 с пакетом обновления 1 (SP1)  | Включает все функции, Exchange 2010 г. В 2010 Exchange 2010 г. были представлены следующие функции:  <ul><li>  Создание, извлечение и изменение правил "Входящие"</li><li>Программный доступ к архивным почтовым ящикам</li><li>Действия разговоров</li><li>Уведомления об обходе брандмауэра</li><li>Улучшенные функции администрирования</li><li>Улучшенная поддержка смешанной версии</li><li>Поддержка защиты от регулирования</li><li>Управление доступом приложений к EWS</li><li>Поддержка проверки подлинности сертификатов клиента</li></ul> |
|Exchange 2010  | Включает все функции, Exchange 2007 sp1. В начальной версии выпуска Exchange 2010 г. были представлены следующие функции: <ul> <li>  Полный частный список рассылки</li><li>Объекты конфигурации пользователей</li><li>Связанные элементы папки</li><li>Отслеживание сообщений</li><li>Единая система обмена сообщениями</li><li>Автообнаружение SOAP  </li><li>Расширенная поддержка часовой зоны</li><li>Сведения о доступности ресурсов комнат</li><li>Индексация поиска</li><li>Доступ к мусорным контейнерам</li><li>Сведения о mailTips</li></ul> |
|Exchange 2007 SP1  | Включает все функции, Exchange 2007 г. В 2007 Exchange 2007 г. были представлены следующие функции:  <ul><li>  Управление делегированием</li><li>Разрешения для папок</li><li>Общедоступные папки</li><li>Почтовые элементы</li><li>Преобразование ID</li></ul> |
|Exchange 2007  | Следующие функции были представлены в начальной версии Exchange 2007 г.:  <ul><li>  Полный доступ к пунктам, папкам и вложениям (создание, получить, обновить, удалить)</li><li>Доступность</li><li>Вне Office параметров</li><li>Уведомления</li><li>Синхронизация</li><li>Разрешение имен</li><li>Расширение списка рассылки (DL)</li><li>Поиск</li></ul> |
   
## <a name="see-also"></a>См. также

- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
- [Переход на технологии Exchange](../migrating-to-exchange-online-and-exchange-2013-technologies.md)
- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
    

