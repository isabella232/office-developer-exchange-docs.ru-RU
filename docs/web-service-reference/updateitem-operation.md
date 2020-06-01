---
title: Операция UpdateItem
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
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459393"
---
# <a name="updateitem-operation"></a>Операция UpdateItem

Операция **UpdateItem** используется для изменения свойств существующего элемента в хранилище Exchange. 
  
## <a name="remarks"></a>Примечания

Для элемента можно выполнить три основные действия по обновлению. В следующей таблице перечислены действия, которые можно выполнить.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Error  <br/> |Добавляет данные к существующему свойству. Это действие сохранит текущие данные. Append не применяется ко всем свойствам.  <br/> |
|Set  <br/> |Заменяет данные для свойства, если свойство содержит данные, или создает свойство и задает его значение, если свойство не существует. Действие Set применяется только к записываемым свойствам.  <br/> |
|Удалить  <br/> |Удаляет свойство из элемента. Это отличается от присвоения свойству пустого значения. По завершении этого действия свойство для элемента не существует. DELETE применяется только к записываемым свойствам.  <br/> |
   
Вызов **UpdateItem** можно использовать для изменения одного или нескольких элементов и одного или нескольких свойств каждого элемента. Элемент [итемчанжес](itemchanges.md) содержит все изменения, которые необходимо выполнить в рамках этого вызова. Элемент [итемчанже](itemchange.md) , являющийся дочерним по отношению к элементу [итемчанжес](itemchanges.md) , представляет изменения, которые необходимо выполнить для одного элемента. Элемент [итемчанже](itemchange.md) содержит набор действий обновления, которые можно выполнить для одного элемента. Эти изменения включены в элемент [Updates (Item)](updates-item.md) . Элемент [ItemId](itemid.md) определяет обновляемый элемент. Чтобы обновить несколько свойств элемента, необходимо предоставить [сетитемфиелд](setitemfield.md), [аппендтоитемфиелд](appendtoitemfield.md)или [делетеитемфиелд](deleteitemfield.md) для каждого свойства, для которого требуется обновление. 
  
> [!NOTE]
> Действия по обновлению применяются в том порядке, в котором они указаны. 
  
Для каждого изменения необходимо указать путь к свойству, которое необходимо изменить, и представление этого элемента с новым значением. Действие DELETE слегка отличается от того, что требуется только путь к удаляемому свойству. Для действий Set и Append указанный путь должен относиться к тому же свойству, которое задается в представлении элемента. Если они отличаются, будет возвращена ошибка.
  
Для операции **UpdateItem** можно задать время [начала](start.md) и [окончания](end-ex15websvcsotherref.md) для элемента хранилища Exchange. В запросе **UpdateItem** время [начала](start.md) может быть задано без указания времени [окончания](end-ex15websvcsotherref.md) . Это может привести к ошибке, если время [начала](start.md) позже времени [окончания](end-ex15websvcsotherref.md) . Имейте в виду, что клиентские приложения должны настроить время [окончания](end-ex15websvcsotherref.md) при изменении времени [начала](start.md) , чтобы сохранить длительность. 
  
Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом основного календаря, свойство [митингтимезоне](meetingtimezone.md) должно быть задано операцией **UpdateItem** для сохранения исходного часового пояса элемента календаря. 
  
## <a name="setitemfield-request-example"></a>Пример запроса Сетитемфиелд

### <a name="description"></a>Описание

В приведенном ниже примере запроса **UpdateItem** показано, как задать свойство "чувствительность" для элемента. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="setitemfield-request-elements"></a>Элементы запроса Сетитемфиелд

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [итемчанжес](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [сетитемфиелд](setitemfield.md)
    
- [фиелдури](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Пример запроса Аппендтоитемфиелд

### <a name="description"></a>Описание

В приведенном ниже примере запроса **UpdateItem** показано, как добавить текст в свойство Body элемента. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Действие Append поддерживается следующими свойствами:
  
- **сообщение: ReplyTo**
    
- **элемент: Body**
    
- Все свойства коллекции получателей и участников
    
Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="appendtoitemfield-request-elements"></a>Элементы запроса Аппендтоитемфиелд

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [итемчанжес](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [аппендтоитемфиелд](appendtoitemfield.md)
    
- [фиелдури](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Body](body.md)
    
## <a name="deleteitemfield-request-example"></a>Пример запроса Делетеитемфиелд

### <a name="description"></a>Описание

В следующем примере запроса **UpdateItem** показано, как удалить свойство элемента. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="deleteitemfield-request-elements"></a>Элементы запроса Делетеитемфиелд

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [итемчанжес](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [делетеитемфиелд](deleteitemfield.md)
    
- [фиелдури](fielduri.md)
    
## <a name="successful-response-example"></a>Пример успешного ответа

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос **UpdateItem** . 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатеитемреспонсе](updateitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [упдатеитемреспонсемессаже](updateitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Идентификатор](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция UpdateItem (Task)](updateitem-operation-task.md)
  
[Операция UpdateItem (Contact)](updateitem-operation-contact.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Обновление задач](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

