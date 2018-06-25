---
title: Операции CreateItem (задача)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: Операции CreateItem создает элементы задачи в хранилище Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761896"
---
# <a name="createitem-operation-task"></a>Операции CreateItem (задача)

Операции CreateItem создает элементы задачи в хранилище Exchange.
  
## <a name="task-createitem-request"></a>Запрос CreateItem задачи

### <a name="description"></a>Описание

В следующем примере запрос CreateItem показано, как создать элемент задачи в почтовом ящике.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Запросы для повторяющихся задач, предоставление при получении на компьютере, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа. Происходят следующие изменения:
  
- Только дата сохраняется для свойства [StartDate (повторения)](startdate-recurrence.md) диапазона повторения задачи. Часть времени усекается. 
    
- Свойство [StartDate (повторения)](startdate-recurrence.md) могут быть изменены в зависимости от шаблона повторения. Например, если повторов задается следующим каждый понедельник, StartDate задано значение 26 октября 2006 г., которая Четверг, корректируется StartDate 30 октября 2006 г., которая является следующий понедельник. 
    
- Если значение свойства [StartDate](startdate.md) задачи, он обновляется в соответствии с [StartDate (повторения)](startdate-recurrence.md) диапазона повторения. Свойство [DueDate](duedate.md) задачи также обновляются на основании нового [StartDate](startdate.md).
    
- Если установлено значение [StartDate](startdate.md) , только свойство [DueDate](duedate.md) обновляется в соответствии с [StartDate (повторения)](startdate-recurrence.md) диапазона повторения. 
    
В следующей таблице перечислены необходимые изменения на сервере клиентского доступа вносятся в повторяющейся задачи, имеющей Task.Recurrence.Pattern каждый понедельник.
  
**Изменения в повторяющейся задачи**

|**Свойство**|**Исходное значение**|**Обновленное значение**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1 января 2006 г.  <br/> |30 октября 2006 г.  <br/> |
|Task.DueDate  <br/> |3 января 2006 г.  <br/> |1 ноября 2006 г.  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 октября 2006 г.  <br/> |30 октября 2006 г.  <br/> |
   
По умолчанию если не указан в целевую папку, элементы задачи создаются в папке задач.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Задача](task.md)
    
- [Subject](subject.md)
    
- [DueDate](duedate.md)
    
- [Состояние](status.md)
    
## <a name="successful-task-createitem-response"></a>Успешные задачу CreateItem ответа

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос CreateItem.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе включены следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Задача](task.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="see-also"></a>См. также



[CreateItem Operation](createitem-operation.md)


[Создание задач](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Обновление задач](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Удаление задачи](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

