---
title: обнаружение электронных данных в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Узнайте об обнаружении электронных данным в EWS в Exchange.
ms.openlocfilehash: 0b4f211e7f8a6ec085fd03ada1cc5a35187106e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512312"
---
# <a name="ediscovery-in-ews-in-exchange"></a>обнаружение электронных данных в веб-службах Exchange

Узнайте об обнаружении электронных данным в EWS в Exchange.
  
eDiscovery — это федераированная веб-служба запроса, которая позволяет внешним приложениям выполнять запросы Exchange данных.
  
Обнаружение состоит из нескольких этапов, включая определение и сохранение ключевых данных, выемку и анализ данных и создание данных в суде. Запросы на обнаружение электронных обнаружений облегчают процесс обнаружения, предоставляя единый рабочий процесс обнаружения Exchange и SharePoint.
  
## <a name="ediscovery-operations"></a>Операции обнаружения электронных данных

Функции eDiscovery, открытые EWS, доступны с помощью операций, введенных в Exchange Online, Exchange Online как часть Office 365, и версий Exchange начиная с Exchange 2013 г. 
  
**Таблица 1. Новые операции для eDiscovery**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Получает сведения о конфигурации для удерживаемого на месте, сохраненных поисков обнаружения и почтовых ящиков, включенных для поиска обнаружения.  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Получает состояние удержания на основе запроса, которое устанавливается с помощью операции [SetHoldOnMailboxes.](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx)  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Извлекает сведения о не индексациях элементов. Это включает идентификатор элемента, код ошибки, описание ошибки при попытке индексации элемента и дополнительные сведения о файле.  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Извлекает количество элементов, которые нельзя индексировать в почтовом ящике.  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Получает список почтовых ящиков, на которые клиент имеет разрешение на поиск или выполнение электронного поиска.  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Поиск элементов в определенных почтовых ящиках, которые соответствуют ключевым словам запроса.  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Задает удержание на основе запроса для элементов.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

