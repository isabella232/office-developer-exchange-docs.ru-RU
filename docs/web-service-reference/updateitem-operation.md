---
title: UpdateItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: Операция UpdateItem используется для изменения свойств существующего элемента в хранилище Exchange.
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840353"
---
# <a name="updateitem-operation"></a>UpdateItem Operation

Операция **UpdateItem** используется для изменения свойств существующего элемента в хранилище Exchange. 
  
## <a name="remarks"></a>Замечания

Можно выполнить три основные обновления действия над элементом. В следующей таблице перечислены действия, которые можно выполнить.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Добавление  <br/> |Добавляет данные существующего свойства. Это действие сохраняет текущих данных. Добавьте не применяется ко всем свойствам.  <br/> |
|Set  <br/> |Заменяет данных для свойства, если свойство содержит данные, или создает свойство и задает его значение, если свойство не существует. Набор действий применима только для записи свойств.  <br/> |
|Удаление  <br/> |Удаляет свойство из элемента. Это отличается от свойства пустое значение. По завершении этого действия свойство не существует для элемента. Удалить применима только для записи свойств.  <br/> |
   
Вызова **UpdateItem** можно использовать для изменения одного или нескольких элементов и одного или нескольких свойств каждого элемента. Элемент [ItemChanges](itemchanges.md) содержит все изменения, которые нужно выполнить в ходе вызова. Элемент [ItemChange](itemchange.md) , дочерний элемент [ItemChanges](itemchanges.md) представляет изменения выполняется на один элемент. Элемент [ItemChange](itemchange.md) содержит набор действия обновления, доступные для отдельных элементов. Эти изменения содержащиеся в элементе [обновлений (элемент)](updates-item.md) . Элемент [ItemId](itemid.md) определяет элемент требуется обновить. Чтобы обновить более одного свойства элемента, [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)или [DeleteItemField](deleteitemfield.md) должно быть указано для каждого свойства, которое требуется обновление. 
  
> [!NOTE]
> Действия Update, применяются в том порядке, в котором они указаны. 
  
Для каждого изменения необходимо указать путь к свойству для изменения и представление такого элемента с его новое значение. Удаление несколько отличается, в том, что является обязательным только путь свойства, подлежащего удалению. Для набора и добавления действия, должен указывать путь, указанный для одного свойства, которое задано в представление элемента. Если они отличаются, будет возвращена ошибка.
  
Операция **UpdateItem** можно задать время [Start](start.md) и [End](end-ex15websvcsotherref.md) объекта хранилища Exchange. В запросе **UpdateItem** можно задать время [начала](start.md) без предоставления время [окончания](end-ex15websvcsotherref.md) . Это может вызвать ошибку, если время [начала](start.md) позднее время [окончания](end-ex15websvcsotherref.md) . Обратите внимание, что клиентских приложений необходимо настроить время [окончания](end-ex15websvcsotherref.md) , при изменении время [начала](start.md) для сохранения во время выполнения. 
  
При обновлении элемента одного календаря стать повторяющегося элемента календаря главных свойство [MeetingTimeZone](meetingtimezone.md) должно быть задано при операции **UpdateItem** для сохранения часового пояса исходного элемента календаря. 
  
## <a name="setitemfield-request-example"></a>Пример запроса SetItemField

### <a name="description"></a>Описание

Приведенный ниже запрос **UpdateItem** показано, как задать свойство уровень конфиденциальности сообщения элемента. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="setitemfield-request-elements"></a>Элементы запроса SetItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Уровень конфиденциальности сообщения](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Пример запроса AppendToItemField

### <a name="description"></a>Описание

В следующем примере запрос **UpdateItem** показано, как добавить текст в свойстве текст элемента. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Следующие свойства поддержка append действия:
  
- **сообщение: ReplyTo**
    
- **основной текст элемента:**
    
- Всех получателей и attendee коллекции свойств
    
Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="appendtoitemfield-request-elements"></a>Элементы запроса AppendToItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Body](body.md)
    
## <a name="deleteitemfield-request-example"></a>Пример запроса DeleteItemField

### <a name="description"></a>Описание

Приведенный ниже запрос **UpdateItem** показано, как удалить свойство элемента. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="deleteitemfield-request-elements"></a>Элементы запроса DeleteItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Пример успешного ответа

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **UpdateItem** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Элементы](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция UpdateItem (задача)](updateitem-operation-task.md)
  
[Операция UpdateItem (контактов)](updateitem-operation-contact.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Обновление контактов](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Обновление задач](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

