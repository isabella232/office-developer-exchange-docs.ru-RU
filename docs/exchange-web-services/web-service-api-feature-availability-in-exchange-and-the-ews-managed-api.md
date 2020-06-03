---
title: Доступность функции веб-службы API в Exchange и в Управляемом API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Сведения о функциях API веб-служб EWS и веб-службах, доступных в каждой версии Exchange и управляемом API EWS.
ms.openlocfilehash: f15cf4784a59c18d1bb9ae20af378baed084acc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529849"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Доступность функции веб-службы API в Exchange и в Управляемом API EWS

Сведения о функциях API веб-служб EWS и веб-службах, доступных в каждой версии Exchange и управляемом API EWS.
  
Клиентские приложения Exchange часто нацелены на множество версий Exchange. По этой причине может потребоваться разрабатывать приложение, чтобы можно было включать и отключать [клиентские компоненты EWS](ews-client-design-overview-for-exchange.md#EWSFeatures) в зависимости от версии Exchange, в которой размещается почтовый ящик пользователя. В этой статье представлены сведения о возможностях API служб в различных версиях Exchange и управляемом API EWS. Используйте эти сведения, чтобы разрабатывать приложение для широкого применения к клиентам с несколькими версиями Exchange. 
  
Для получения подробных сведений о различиях между версиями Exchange просмотрите файлы схемы EWS и связанную [справочную документацию](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx).
  
## <a name="api-features-by-exchange-version"></a>Функции API по версии Exchange
<a name="bk_apifeatures"> </a>

API веб-службы Exchange, в том числе EWS и автообнаружения, разработаны с использованием совместимости с несколькими версиями. Таким образом, приложение, предназначенное для Exchange 2007, также работает и с версиями Exchange, начиная с Exchange 2013, включая Exchange Online и Exchange Online в составе Office 365. 
  
В следующей таблице перечислены функции API, доступные в каждой версии Exchange и версиях управляемого API EWS, начиная с версии 2,0. Так как приложение может ориентироваться на несколько версий Exchange, вам будет полезно знать, какие версии поддерживают функции, реализуемые клиентом. Службу автообнаружения можно использовать для определения того, какая версия Exchange является клиентом для пользователя, что позволяет включать и отключать компоненты в зависимости от того, доступны ли они пользователям.
  
**Таблица 1. Доступность функций веб-служб в версиях Exchange и управляемом API EWS**

|Функция API|Exchange Online (Office 365)|Управляемый API EWS|Exchange 2013|Exchange 2010 с пакетом обновления 2 (SP2)|Exchange 2010 с пакетом обновления 1 (SP1)|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Разрешение неоднозначных имен  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Управление приложениями для Outlook  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Доступ к архивному почтовому ящику](archiving-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Служба автообнаружения (POX)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Служба автообнаружения (SOAP)](autodiscover-for-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Автоматические ответы (отсутствие на работе)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Доступность  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Доступность (комнаты)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Массовый перевод  <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> ||||
|Группы контактов  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Управление беседами  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Точность значений даты и времени  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|Управление делегированием  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Расширение списка рассылки  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Доступ к корзине](deleting-items-by-using-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Обнаружение электронных данных](ediscovery-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|Расширенные Часовые пояса  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|Разрешения для папок  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Преобразование идентификатора](ews-identifiers-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Управление папкой "Входящие"](inbox-management-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|[Доступ к элементам и папкам](folders-and-items-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[События почтового ящика (Опрашивающая и извещающая)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[События почтовых ящиков (потоковая передача)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Подсказки  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||||
|Срок действия пароля  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||||
|[Фиктивные пользователи](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|Размещение элементов  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|[Доступ к общедоступным папкам](public-folder-access-with-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> ||
|Политики хранения  <br/> |X  <br/> |X  <br/> |X  <br/> ||||||
|[Поиск (индексированный)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Поиск (магазин)](search-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Синхронизация](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|[Единая база контактов](people-and-contacts-in-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
|[Веб-служба единой системы обмена сообщениями](https://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X  <br/> ||X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |
|Единая система обмена сообщениями (на основе EWS)  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Объекты конфигурации пользователя](persistent-application-settings-in-ews-in-exchange.md) <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |X  <br/> |||
|[Фотографии пользователя](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X  <br/> ||X  <br/> ||||||
   
Дополнительные сведения о функциях веб-служб, доступных в различных версиях Exchange, можно найти, прочитав [операции EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), [службу автообнаружения](https://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)и [методы ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Дополнительные сведения
<a name="bk_apifeatures"> </a>

Если вы хотите глубже изучить конкретные различия между версиями Exchange, выполните одно из следующих действий.
  
- Изучите [схему EWS](https://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) , чтобы более подробно изучить различия между каждой версией EWS. 
    
- Скачайте [евседитор](http://ewseditor.codeplex.com/). Вы можете использовать Евседитор, чтобы указать разные целевые версии схемы и отправляют запросы на основе целевой версии схемы.
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Новые возможности в веб-службах EWS и других веб-службах в Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

