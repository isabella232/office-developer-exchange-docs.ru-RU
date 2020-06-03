---
title: Операция MoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: Операция MoveItem используется для перемещения одного или нескольких элементов в одну целевую папку.
ms.openlocfilehash: 6a455e483ad2e5c84b91cfaa7562f4f1ec46a112
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465683"
---
# <a name="moveitem-operation"></a>Операция MoveItem

Операция **MoveItem** используется для перемещения одного или нескольких элементов в одну целевую папку. 
  
## <a name="moveitem-request-example"></a>Пример запроса MoveItem

### <a name="description"></a>Description

В приведенном ниже примере запроса **MoveItem** показано, как переместить элемент в папку "Черновики". 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Элемент [тофолдерид](tofolderid.md) указывает папку, в которую будут перемещены элементы. Обратите внимание, что все элементы, перечисленные в коллекции [итемидс](itemids.md) , будут находиться в конечной папке. Для размещения элементов в разных папках назначения необходимо выполнить отдельные вызовы **MoveItem** . 
  
> [!NOTE]
> Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [MoveItem](moveitem.md)
    
- [тофолдерид](tofolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="moveitem-response-example"></a>Пример отклика MoveItem

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **MoveItem** . 
  
В ответном сообщении возвращается идентификатор элемента нового элемента. Идентификаторы элементов не возвращаются в ответах на операции **MoveItem** для нескольких почтовых ящиков или почтовых ящиков в общедоступных папках. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Если перемещение прошло успешно, операция **MoveItem** будет указывать на успешное выполнение. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [мовеитемреспонсе](moveitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [мовеитемреспонсемессаже](moveitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

