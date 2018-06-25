---
title: MoveItem Operation
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
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834492"
---
# <a name="moveitem-operation"></a>MoveItem Operation

Операция **MoveItem** используется для перемещения одного или нескольких элементов в одну целевую папку. 
  
## <a name="moveitem-request-example"></a>Пример запроса MoveItem

### <a name="description"></a>Описание

Приведенный ниже запрос **MoveItem** показано перемещение элемента в папке "Черновики". 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Элемент [ToFolderId](tofolderid.md) указывает папку, в который перемещается элементы. Обратите внимание на то, что все элементы, перечисленные в коллекции [что ItemID](itemids.md) окажутся в папке назначения. Необходимо включить для отдельных вызовов **MoveItem** размещение элементов в разных конечные папки. 
  
> [!NOTE]
> Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [MoveItem](moveitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Что ItemID](itemids.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="moveitem-response-example"></a>Пример ответа MoveItem

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **MoveItem** . 
  
Идентификатор нового элемента, возвращается в сообщении ответа. Идентификаторы элементов не возвращаются в ответ для нескольких почтовых или почтовых ящиков операциям **MoveItem** общей папки. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Операция **MoveItem** содержатся сведения о успешное перемещение выполнено успешно. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [MoveItemResponse](moveitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MoveItemResponseMessage](moveitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Элементы](items.md)
    
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

