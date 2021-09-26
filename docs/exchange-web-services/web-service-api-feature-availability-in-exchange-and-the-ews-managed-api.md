---
title: Доступность функции веб-службы API в Exchange и в Управляемом API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Узнайте, какие функции API EWS и веб-служб доступны в каждой версии Exchange и управляемом API EWS.
ms.openlocfilehash: 6fc0c40410be543b149885c7b0785a2c6c8828af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544474"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Доступность функции веб-службы API в Exchange и в Управляемом API EWS

Узнайте, какие функции API EWS и веб-служб доступны в каждой версии Exchange и управляемом API EWS.
  
Exchange клиентские приложения часто ориентированы на многие версии Exchange. По этой причине может потребоваться создать приложение таким образом, чтобы можно было включить и отключить функции клиента [EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) на основе версии Exchange, в которой размещен почтовый ящик пользователей. В этой статье представлены сведения о том, какие функции API службы доступны в различных Exchange и управляемом API EWS. Используйте эти сведения для разработки приложения для широкого применения к клиентам, работающим с несколькими версиями Exchange. 
  
Подробные сведения о различиях между версиями Exchange описаны в файлах схемы EWS и [связанной справочной документации.](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx)
  
## <a name="api-features-by-exchange-version"></a>Функции API по Exchange версии
<a name="bk_apifeatures"> </a>

API Exchange службы, включая EWS и autodiscover, разработаны с учетом многоверсийной совместимости. Поэтому приложение, которое нацелено на Exchange 2007 г., также работает с версиями Exchange, начиная с Exchange 2013 г., включая Exchange Online и Exchange Online как часть Office 365. 
  
В следующей таблице указывается, какие функции API доступны в каждой версии Exchange и версии управляемого API EWS начиная с версии 2.0. Так как приложение может быть ориентировано на несколько Exchange, вам будет полезно узнать, какие версии поддерживают функции, реализуемые клиентом. Вы можете использовать службу автообнаружение, чтобы узнать, какая версия Exchange клиентских целей для пользователя, чтобы включить и отключить функции в зависимости от того, доступны ли они пользователям.
  
**Таблица 1. Доступность функций веб-служб в версиях Exchange и управляемом API EWS**

|Функция API|Exchange Online (Office 365)|Управляемый API EWS|Exchange 2013|Exchange 2010 с пакетом обновления 2 (SP2)|Exchange 2010 с пакетом обновления 1 (SP1)|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Неоднозначное разрешение имен  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Приложения для Outlook управления  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Доступ к архивным почтовым ящикам](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Автоматическое открытие (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Автонаружить (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Автоматические ответы (OOF)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Доступность  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Доступность (комнаты)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Массовый перенос  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Группы контактов  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Управление разговорами  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Точность DateTime  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Управление делегированием  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Расширение списка рассылки  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Доступ к мусорным контейнерам](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Обнаружение электронных данных](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Расширенные часовые пояса  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Разрешения для папок  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Преобразование идентификатора](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Управление папкой "Входящие"](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Доступ к элементам и папкам](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[События почтовых ящиков (тянуть и толкать)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[События почтовых ящиков (потоковая передача)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Mailtips  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Срок действия пароля  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Personas](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Почтовые элементы  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Доступ к общедоступным папкам](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Политики хранения  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Поиск (индексация)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Поиск (магазин)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Синхронизация](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Единая база контактов](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Единая веб-служба обмена сообщениями](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Единая система обмена сообщениями (на основе EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Объекты конфигурации пользователя](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Фотографии пользователя](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Дополнительные сведения о веб-службах, доступных в различных версиях Exchange, вы можете найти, [](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)прочитав о операциях [EWS,](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx)службе автообнаружения и методах [ExchangeService.](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx)
  
## <a name="to-learn-more"></a>Дополнительные
<a name="bk_apifeatures"> </a>

Если вы хотите глубже разобраться в конкретных различиях между Exchange версиями, вы можете сделать любой из следующих вариантов:
  
- Ознакомьтесь [с схемой EWS,](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) чтобы более подробно изучить различия между каждой версией EWS. 
    
- Скачайте [EWSEditor](http://ewseditor.codeplex.com/). Вы можете использовать EWSEditor для указания различных версий целевой схемы и отправки запросов на основе целевой версии схемы.
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Что нового в EWS и других веб-службах в Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

