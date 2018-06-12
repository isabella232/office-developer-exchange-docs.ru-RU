---
title: Операция DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 3e26c416-fa12-476e-bfd2-5c1f4bb7b348
description: Операция DeleteItem удаляет элементы в хранилище Exchange.
ms.openlocfilehash: 87d7853daa5db0cd87b3f6469c228a584b4d9caf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762043"
---
# <a name="deleteitem-operation"></a>Операция DeleteItem

Операция **DeleteItem** удаляет элементы в хранилище Exchange. 
  
> [!NOTE]
> Ответ на ошибку, которая включает в себя код ошибки ErrorCannotDeleteObject будут возвращены для выполнения операции **DeleteItem** при попытке удалить элемент в почтовом ящике участника путем установки для параметра MoveToDeletedItems DisposalType делегата. Чтобы удалить элемент путем перемещения в папку «Удаленные», делегата необходимо использовать [MoveItem операции](moveitem-operation.md). 
  
## <a name="deleteitem-request-example"></a>Пример запроса DeleteItem

### <a name="description"></a>Описание

В следующем примере запрос **DeleteItem** показано, как выполнить окончательного удаления элемента из почтового ящика. 
  
> [!NOTE]
> Идентификатор элемента был усечен, чтобы сохранить удобочитаемость. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [DeleteItem](deleteitem.md)
    
- [Что ItemID](itemids.md)
    
- [Идентификатор элемента](itemid.md)
    
Чтобы найти другие параметры для запроса **DeleteItem** операции, изучите иерархия схемы. Начать с [DeleteItem](deleteitem.md) элемента. 
  
## <a name="successful-deleteitem-response"></a>Успешные DeleteItem ответа

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **DeleteItem** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteItemResponse](deleteitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
Чтобы найти другие параметры в сообщении ответа **DeleteItem** операции, изучите иерархия схемы. Запустите в элементе [DeleteItemResponse](deleteitemresponse.md) . 
  
## <a name="deleteitem-error-response"></a>Ошибка DeleteItem ответа

### <a name="description"></a>Описание

В следующем примере показано возврату ошибки **DeleteItem** запрос. Ошибка была создана, поскольку операции пытались удалить элемент, который не найден в хранилище Exchange. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </DeleteItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteItemResponse](deleteitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteItemResponseMessage](deleteitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Чтобы найти другие параметры в сообщении об ошибке ответа **DeleteItem** операции, изучите иерархия схемы. Запустите в элементе [DeleteItemResponse](deleteitemresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление контактов](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [Удаление сообщений электронной почты](http://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [Удаление задачи](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

