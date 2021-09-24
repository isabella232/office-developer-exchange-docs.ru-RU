---
title: Операция CreateItem (задача)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: Операция CreateItem создает элементы задач в Exchange магазине.
ms.openlocfilehash: 814a32e82cd5c1c95be252d1b53387741898dd40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510261"
---
# <a name="createitem-operation-task"></a>Операция CreateItem (задача)

Операция CreateItem создает элементы задач в Exchange магазине.
  
## <a name="task-createitem-request"></a>Запрос на создание задач

### <a name="description"></a>Описание

В следующем примере запроса CreateItem показано, как создать элемент задачи в почтовом ящике.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
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

Запросы на повторяющиеся задачи изменяются, когда они получаются на компьютере, который Microsoft Exchange Server 2007, где установлена роль сервера клиентского доступа. Происходят следующие изменения:
  
- Для свойства [StartDate (Recurrence)](startdate-recurrence.md) диапазона повторяемости задачи сохранена только дата. Временная часть усечена. 
    
- Свойство [StartDate (Recurrence)](startdate-recurrence.md) может быть скорректировано в зависимости от шаблона повторения. Например, если шаблон повторения указывается как каждый понедельник, а startDate — 26 октября 2006 г., то есть четверг, StartDate корректируется до 30 октября 2006 г., то есть на следующий понедельник. 
    
- Если [задано свойство StartDate](startdate.md) задачи, оно обновляется в соответствие с [диапазоном повторения StartDate (Recurrence).](startdate-recurrence.md) Свойство [DueDate](duedate.md) задачи также обновляется на основе нового [StartDate.](startdate.md)
    
- Если [startDate](startdate.md) не установлен, обновляется только свойство [DueDate,](duedate.md) чтобы соответствовать [диапазону повторения StartDate (Recurrence).](startdate-recurrence.md) 
    
В следующей таблице показаны изменения, которые сервер клиентского доступа вносит в повторяемую задачу, которая имеет task.Recurrence.Pattern каждого понедельника.
  
**Изменения в повторяющейся задаче**

|**Property**|**Исходное значение**|**Обновленное значение**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1 января 2006 г.  <br/> |30 октября 2006 г.  <br/> |
|Task.DueDate  <br/> |3 января 2006 г.  <br/> |1 ноября 2006 г.  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 октября 2006 г.  <br/> |30 октября 2006 г.  <br/> |
   
По умолчанию, если папка назначения не указана, элементы задач создаются в папке Задачи.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Задача](task.md)
    
- [Тема](subject.md)
    
- [DueDate](duedate.md)
    
- [Состояние](status.md)
    
## <a name="successful-task-createitem-response"></a>Успешный ответ createItem задачи

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateItem.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В ответ включены следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Задача](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция CreateItem](createitem-operation.md)


[Создание задач](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Обновление задач](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Удаление задач](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

