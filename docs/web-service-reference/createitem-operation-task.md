---
title: Операция CreateItem (задача)
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
description: Операция CreateItem создает элементы Task в хранилище Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761896"
---
# <a name="createitem-operation-task"></a>Операция CreateItem (задача)

Операция CreateItem создает элементы Task в хранилище Exchange.
  
## <a name="task-createitem-request"></a>Запрос CreateItem задачи

### <a name="description"></a>Описание

В приведенном ниже примере запроса CreateItem показано, как создать элемент задачи в почтовом ящике.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

Запросы на повторяющиеся задачи изменяются при их получении на компьютере под управлением Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа. Происходят следующие изменения:
  
- Только дата сохраняется в свойстве [StartDate (повторение)](startdate-recurrence.md) для интервала повторения задачи. Часть времени усекается. 
    
- Свойство [StartDate (повторение)](startdate-recurrence.md) можно изменить в зависимости от расписания повторения. Например, если расписание повторения задано как каждый понедельник, а значение StartDate равно 26 октября 2006 г., то есть четверг, Дата начала StartDate составляет 30 октября 2006, то есть на следующий понедельник. 
    
- Если свойство [StartDate](startdate.md) задания задано, оно обновляется в соответствующем поле [StartDate (повторение)](startdate-recurrence.md) диапазона повторения. Свойство [DueDate](duedate.md) задачи также обновляется в соответствии с новым [StartDate](startdate.md).
    
- Если [StartDate](startdate.md) не задан, обновляется только свойство [DueDate](duedate.md) , которое будет иметь значение [StartDate (повторение)](startdate-recurrence.md) диапазона повторения. 
    
В следующей таблице показаны изменения, которые сервер клиентского доступа выполняет с повторяющейся задачей, у которой есть задача. повторять. шаблон каждого понедельника.
  
**Изменение повторяющейся задачи**

|**Свойство**|**Исходное значение**|**Обновленное значение**|
|:-----|:-----|:-----|
|Task. StartDate  <br/> |1 января 2006 г.  <br/> |30 октября 2006 г.  <br/> |
|Task. DueDate  <br/> |3 января 2006 г.  <br/> |1 ноября 2006 г.  <br/> |
|Task. повторяющуюся. Range. StartDate  <br/> |26 октября 2006 г.  <br/> |30 октября 2006 г.  <br/> |
   
По умолчанию, если папка назначения не указана, элементы задач создаются в папке "задачи".
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [Тема](subject.md)
    
- [DueDate](duedate.md)
    
- [Состояние](status.md)
    
## <a name="successful-task-createitem-response"></a>Отклик об успешном выполнении операции CreateItem

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

В ответ включаются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеитемреспонсе](createitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеитемреспонсемессаже](createitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [Идентификатор](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция CreateItem](createitem-operation.md)


[Создание задач](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Обновление задач](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Удаление задач](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

