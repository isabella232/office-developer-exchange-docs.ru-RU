---
title: обнаружение электронных данных в веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3128419f-dd5f-46d2-bb0d-0940738d0bb6
description: Сведения об обнаружении электронных данных в EWS в Exchange.
ms.openlocfilehash: 48e3fdb3a2f21f7dcfcb7eed21b586e099b249a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456096"
---
# <a name="ediscovery-in-ews-in-exchange"></a>обнаружение электронных данных в веб-службах Exchange

Сведения об обнаружении электронных данных в EWS в Exchange.
  
Обнаружение электронных данных — это веб-служба федеративных запросов, которая позволяет внешним приложениям выполнять запросы данных Exchange.
  
Обнаружение состоит из нескольких этапов, в том числе определения и сохранения данных ключей, отбора и просмотра данных, а также создания данных в суд. запросы eDiscovery упрощают процесс обнаружения, предоставляя единый рабочий процесс обнаружения в Exchange и SharePoint.
  
## <a name="ediscovery-operations"></a>Операции обнаружения электронных данных

Функции обнаружения электронных данных, предоставляемые EWS, доступны с помощью операций, представленных в Exchange Online, Exchange Online в составе Office 365, и версий Exchange, начинающихся с Exchange 2013. 
  
**Таблица 1. Новые операции обнаружения электронных данных**

|**Имя операции**|**Описание**|
|:-----|:-----|
|[GetDiscoverySearchConfiguration](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) <br/> |Получает сведения о конфигурации для удержаний на месте, сохраненных поисков и почтовых ящиков, которые включены для поиска при обнаружении.  <br/> |
|[GetHoldOnMailboxes](https://msdn.microsoft.com/library/9157f329-80b4-4cd0-a158-378064966ae6%28Office.15%29.aspx) <br/> |Получает состояние хранения на основе запроса, которое задается с помощью [операции SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx).  <br/> |
|[GetNonIndexableItemDetails](https://msdn.microsoft.com/library/9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a%28Office.15%29.aspx) <br/> |Получает сведения о элементах, которые не удается индексировать. Это относится только к идентификатору элемента, к коду ошибки, описанию ошибки, при попытке индексирования элемента и дополнительной информации о файле.  <br/> |
|[GetNonIndexableItemStatistics](https://msdn.microsoft.com/library/ed077877-9d98-4434-b8b6-a4a905e7f7a6%28Office.15%29.aspx) <br/> |Получает количество элементов, которые не удается индексировать в почтовом ящике.  <br/> |
|[GetSearchableMailboxes](https://msdn.microsoft.com/library/47f8ff57-4835-4d2d-9136-44afb31a4cbe%28Office.15%29.aspx) <br/> |Получает список почтовых ящиков, у которых у клиента есть разрешение на поиск и выполнение обнаружения электронных данных.  <br/> |
|[SearchMailboxes](https://msdn.microsoft.com/library/8a67c1d8-d021-4e68-aa62-35f7d9c2edc7%28Office.15%29.aspx) <br/> |Ищет элементы в определенных почтовых ящиках, которые совпадают с ключевыми словами запроса.  <br/> |
|[SetHoldOnMailboxes](https://msdn.microsoft.com/library/9015a0d8-3495-461b-aa79-797d23169585%28Office.15%29.aspx) <br/> |Задает для элементов удержание на основе запроса.  <br/> |
   
## <a name="see-also"></a>См. также

- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
    
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    

