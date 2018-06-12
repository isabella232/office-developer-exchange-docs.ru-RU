---
title: Доступность функций API службы Web в Exchange и управляемый API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 07d3e6e8-d549-4ad7-baa4-bc531dfb7dd2
description: Узнайте, какие веб-служб Exchange и веб-служба функции API, доступные в каждой версией Exchange и управляемый API веб-служб Exchange.
ms.openlocfilehash: d19ab062c8d418e373e8268b1ab039e5436e71bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761250"
---
# <a name="web-service-api-feature-availability-in-exchange-and-the-ews-managed-api"></a>Доступность функций API службы Web в Exchange и управляемый API веб-служб Exchange

Узнайте, какие веб-служб Exchange и веб-служба функции API, доступные в каждой версией Exchange и управляемый API веб-служб Exchange.
  
Клиентские приложения Exchange часто предназначены для многих версий Exchange. По этой причине можно разработать приложение таким образом, можно включить [функции клиентов веб-служб Exchange](ews-client-design-overview-for-exchange.md#EWSFeatures) и отключает зависимости от версии, на котором размещен почтовый ящик пользователей Exchange. В этой статье представлены сведения о том, какие функции API службы, доступные в различных версиях Exchange и управляемый API веб-служб Exchange. Используйте эту информацию для разработки приложения для применения в широком для клиентов, использующих несколько версий Exchange. 
  
Получить подробные сведения о различиях между версиями Exchange просмотрите файлы схемы веб-служб Exchange и связанные [справочную документацию](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx).
  
## <a name="api-features-by-exchange-version"></a>Функции API, версия Exchange
<a name="bk_apifeatures"> </a>

Веб-службы Exchange интерфейсов API, включая веб-служб Exchange и службы автообнаружения, разработанных с учетом совместимости версий. Таким образом приложения, предназначенное для Exchange 2007 также работает с версии Exchange, начиная с Exchange 2013, включая Exchange Online и Exchange Online в составе Office 365. 
  
В этой таблице перечислены функций API, доступных в каждой версии Exchange и версиям управляемый API EWS начиная с версии 2.0. Так как приложение может использовать несколько версий Exchange, могут быть полезны для вам необходимо знать, какие версии поддерживают компоненты, реализующий вашего клиента. Можно использовать службы автообнаружения для обнаружения версии клиента предназначен для пользователя, чтобы установить включать и отключать функции в зависимости от того, являются ли они доступными для пользователей Exchange.
  
**В таблице 1. Доступность функции службы Web в версиях Exchange и управляемый API веб-служб Exchange**

|Функции API|Exchange Online (Office 365)|Управляемый API EWS|Exchange 2013|Exchange 2010 SP2|Exchange 2010 SP1|Exchange 2010|Exchange 2007 SP1|Exchange 2007|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|Разрешения неоднозначных псевдонимов  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Приложения для управления Outlook  <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|[Доступ к почтовому ящику архива](archiving-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|[Автообнаружение (POX)](autodiscover-for-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Автообнаружение (SOAP)](autodiscover-for-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Автоматические ответы (OOF)  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Availability  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Доступность (комнат)  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Массовое передачи  <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> ||||
|Группы контактов  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Управление преобразованием  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Точность даты и времени  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||||
|Делегирование управления  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|Раскрытие списка рассылки  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Access корзины](deleting-items-by-using-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[обнаружение электронных данных](ediscovery-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|Усовершенствованные часовые пояса  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|Разрешения для папки  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Идентификатор преобразования](ews-identifiers-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Управление папки "Входящие"](inbox-management-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|[Папки и элемента доступа](folders-and-items-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[События почтового ящика (и)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[События почтового ящика (потоковое воспроизведение)](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Почтовые подсказки  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||||
|Истечение срока действия пароля  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||||
|[Действующие лица](people-and-contacts-in-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
|Элементы  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|[Доступ к общим папкам](public-folder-access-with-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> ||
|Политики хранения  <br/> |X   <br/> |X   <br/> |X   <br/> ||||||
|[Поиск (индексами)](search-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Поиск (внутренний)](search-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Синхронизация](mailbox-synchronization-and-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|[Единое хранилище контактов](people-and-contacts-in-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
|[Единая система обмена сообщениями веб-службы](http://msdn.microsoft.com/library/83afea8a-c716-41df-9eb2-e1000357afb6%28Office.15%29.aspx) <br/> |X   <br/> ||X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |
|Единая система обмена сообщениями (на основе веб-служб Exchange)  <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Настройка пользовательских объектов](persistent-application-settings-in-ews-in-exchange.md) <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |X   <br/> |||
|[Фотографии пользователя](how-to-get-user-photos-by-using-ews-in-exchange.md) <br/> |X   <br/> ||X   <br/> ||||||
   
Можно найти дополнительные сведения о веб-компонентов службы, доступные в различных версиях Exchange при чтении о [операции EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), [службы автообнаружения](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)и [ExchangeService методы](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice_methods%28v=exchg.80%29.aspx).
  
## <a name="to-learn-more"></a>Для получения дополнительных сведений
<a name="bk_apifeatures"> </a>

Если вы хотите пойти еще дальше понять различия между версиями Exchange, можно выполните любые из следующих действий.
  
- Обзор [схемы веб-служб Exchange](http://msdn.microsoft.com/library/6c969133-6036-448b-af39-a3caf9917e98%28Office.15%29.aspx) для изучения различия между каждой версии веб-служб Exchange более подробно. 
    
- Загрузите [EWSEditor](http://ewseditor.codeplex.com/). EWSEditor можно использовать для указания различных целевых версий схемы и отправлять запросы на основании версии схемы целевой.
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Новые возможности веб-служб Exchange и другие веб-службы в Exchange](whats-new-in-ews-and-other-web-services-in-exchange.md)
    

