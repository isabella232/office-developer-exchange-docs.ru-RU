---
title: Операция UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: Операция UpdateItem используется для изменения свойств существующего элемента в Exchange магазине.
ms.openlocfilehash: 6ac09c24c13efff8053fc605ec2c0e6cf2957429
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514062"
---
# <a name="updateitem-operation"></a>Операция UpdateItem

Операция **UpdateItem** используется для изменения свойств существующего элемента в Exchange магазине. 
  
## <a name="remarks"></a>Заметки

Вы можете выполнить три основных действия обновления элемента. В следующей таблице перечислены действия, которые можно выполнить.
  
|**Действие**|**Описание**|
|:-----|:-----|
|Приложение  <br/> |Добавляет данные в существующее свойство. Это действие сохраняет текущие данные. Приложение не применяется к всем свойствам.  <br/> |
|Set  <br/> |Заменяет данные для свойства, если свойство содержит данные, или создает свойство и задает его значение, если свойство не существует. Действие набора применимо только к рукописным свойствам.  <br/> |
|Удалить  <br/> |Удаляет свойство из элемента. Это отличается от установки свойства на пустое значение. По завершению этого действия свойство не существует для элемента. Удаление применимо только к writable свойствам.  <br/> |
   
Вызов **UpdateItem** можно использовать для изменения одного или более элементов и одного или более свойств каждого элемента. Элемент [ItemChanges](itemchanges.md) содержит все изменения, которые должны выполняться в рамках этого вызова. Элемент [ItemChange,](itemchange.md) дитя элемента [ItemChanges,](itemchanges.md) представляет изменения, выполняемые на одном элементе. Элемент [ItemChange](itemchange.md) содержит набор действий обновления, которые можно выполнить на одном элементе. Эти изменения содержатся в [элементе Updates (Item).](updates-item.md) Элемент [ItemId](itemid.md) определяет элемент для обновления. Чтобы обновить несколько свойств элемента, для каждого свойства, требуемого обновления, необходимо уполномочить [SetItemField,](setitemfield.md) [AppendToItemField](appendtoitemfield.md)или [DeleteItemField.](deleteitemfield.md) 
  
> [!NOTE]
> Действия обновления применяются в порядке, в котором они указаны. 
  
Для каждого изменения необходимо указать путь изменения свойства и представление этого элемента с его новым значением. Действие удаления немного отличается тем, что требуется только путь удаляемого свойства. Для действий набора и приложения указанный путь должен ссылаться на то же свойство, которое задано в представлении элемента. Если они отличаются, будет возвращена ошибка.
  
Операция **UpdateItem** может установить [](end-ex15websvcsotherref.md) [время](start.md) начала и окончания элемента Exchange магазина. В **запросе UpdateItem** [можно](start.md) установить время запуска без установки [конечного](end-ex15websvcsotherref.md) времени. Это может привести к ошибке, [если](start.md) время начала более позднее, чем [время окончания.](end-ex15websvcsotherref.md) Следует помнить, что клиентские [](end-ex15websvcsotherref.md) приложения должны [](start.md) настроить время окончания при смене времени начала, чтобы сохранить продолжительность. 
  
Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом календаря, свойство [MeetingTimeZone](meetingtimezone.md) должно быть задано операцией **UpdateItem,** чтобы сохранить исходный часовой пояс элемента календаря. 
  
## <a name="setitemfield-request-example"></a>Пример запроса SetItemField

### <a name="description"></a>Описание

В следующем примере **запроса UpdateItem** показано, как установить свойство чувствительности для элемента. 
  
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

Идентификатор элемента и ключ изменения были сокращены для сохранения читаемости.
  
### <a name="setitemfield-request-elements"></a>Элементы запроса SetItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Пример запроса AppendToItemField

### <a name="description"></a>Описание

В следующем примере **запроса UpdateItem** показано, как приложение текста к свойству тела на элементе. 
  
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

Следующие свойства поддерживают действие приложения:
  
- **message:ReplyTo**
    
- **item:Body**
    
- Все свойства коллекции получателей и участников
    
Идентификатор элемента и ключ изменения были сокращены для сохранения читаемости.
  
### <a name="appendtoitemfield-request-elements"></a>Элементы запроса AppendToItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [Основной текст](body.md)
    
## <a name="deleteitemfield-request-example"></a>Пример запроса DeleteItemField

### <a name="description"></a>Описание

В следующем примере **запроса UpdateItem** показано, как удалить свойство элемента. 
  
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

Идентификатор элемента и ключ изменения были сокращены для сохранения читаемости.
  
### <a name="deleteitemfield-request-elements"></a>Элементы запроса DeleteItemField

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Updates (Item)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Пример успешного ответа

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос **UpdateItem.** 
  
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

Идентификатор элемента и ключ изменения были сокращены для сохранения читаемости.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>См. также



[Операция UpdateItem (задача)](updateitem-operation-task.md)
  
[Операция UpdateItem (контакт)](updateitem-operation-contact.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Обновление задач](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

