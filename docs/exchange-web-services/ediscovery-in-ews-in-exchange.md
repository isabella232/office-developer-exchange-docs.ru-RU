---
title: обнаружение электронных данных в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Узнайте об eDiscovery в веб-служб Exchange в Exchange.
ms.openlocfilehash: 6491fdd9f2246870a89bfa89bf7d97b972d67c92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760939"
---
# <a name="ediscovery-in-ews-in-exchange"></a>обнаружение электронных данных в веб-службах Exchange

Узнайте об eDiscovery в веб-служб Exchange в Exchange.
  
обнаружение электронных данных является федеративным запроса веб-службы, которая позволяет внешних приложений для выполнения запросов данных Exchange.
  
Обнаружение включает несколько этапов, включая определение и сохранение данных ключа, отбора вниз и просмотра данных и создания данных в суд. запросов обнаружения электронных данных упростить процесс обнаружения с указанием одного обнаружения рабочего процесса в Exchange и SharePoint.
  
## <a name="ediscovery-operations"></a>Операции обнаружения электронных данных

Функциональные возможности обнаружения электронных данных, взаимодействующий с веб-служб Exchange доступен через операции, введенные в Exchange Online, Exchange Online как часть Office 365 и версии Exchange, начиная с Exchange 2013. 
  
**В таблице 1. Новых операций для обнаружения электронных данных**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Получает данные конфигурации для удержания на месте, сохраненные операций поиска обнаружения и почтовые ящики, которые разрешены для поиска обнаружения.  <br/> |
|[GetHoldOnMailboxes](http://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Получает состояние запроса на удержание, которая задается с помощью [операции SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](http://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Извлекает сведения об элементах, которые не могут быть индексированы. Это включает в себя, но не ограничивается идентификатор элемента, код ошибки, описание ошибки при попытке индексировать элемент, а также дополнительные сведения о файле.  <br/> |
|[GetNonIndexableItemStatistics](http://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Получает число элементов, которые не могут быть индексированы в почтовом ящике.  <br/> |
|[GetSearchableMailboxes](http://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Получает список почтовых ящиков, который имеет разрешение на поиска или обнаружения электронных данных на клиенте.  <br/> |
|[SearchMailboxes](http://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Выполняет поиск элементов в определенных почтовых ящиков, которые соответствуют ключевые слова запроса.  <br/> |
|[SetHoldOnMailboxes](http://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Наборы на основе запроса содержат элементы.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

