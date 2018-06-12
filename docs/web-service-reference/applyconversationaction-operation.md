---
title: Операция ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: Операция ApplyConversationAction задает одноразовый или исполнению действие для всех элементов в беседе. Операция ApplyConversationAction позволяет распределить по категориям, перемещение, копирование, удаление и устанавливать состояние чтения всех элементов в беседе. Действия можно также задать для новых сообщений в беседе.
ms.openlocfilehash: 2a485b84ee87aec2ed807e3f4f0901b83432fa0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761424"
---
# <a name="applyconversationaction-operation"></a>Операция ApplyConversationAction

Операция **ApplyConversationAction** задает одноразовый или исполнению действие для всех элементов в беседе. Операция **ApplyConversationAction** позволяет распределить по категориям, перемещение, копирование, удаление и устанавливать состояние чтения всех элементов в беседе. Действия можно также задать для новых сообщений в беседе. 
  
## <a name="applyconversationaction-request-example"></a>Пример запроса ApplyConversationAction

### <a name="description"></a>Описание

В следующем примере запрос **ApplyConversationAction** показано, как перемещать элементы в указанной беседе в другую папку. Также элементы, добавляемые к беседе будут перемещены в указанную папку. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a>Замечания

Идентификаторы беседы и папки URL-были сокращены, чтобы сохранить удобочитаемость.
  
## <a name="applyconversationaction-response-example"></a>Пример ответа ApplyConversationAction

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **ApplyConversationAction** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Операции EWS в Exchange](ews-operations-in-exchange.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Conversations in EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

