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
description: Операция DeleteItem удаляет элементы из хранилища Exchange.
ms.openlocfilehash: f068e08ef0d0f590c9ed8274f77d4dae9f942995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526937"
---
# <a name="deleteitem-operation"></a>Операция DeleteItem

Операция **DeleteItem** удаляет элементы из хранилища Exchange. 
  
> [!NOTE]
> Если делегат пытается удалить элемент в почтовом ящике участника, задав для Диспосалтипе значение MoveToDeletedItems, возвращается сообщение об ошибке, которое включает код ошибки Еррорканнотделетеобжект для операции **DeleteItem** . Чтобы удалить элемент, переместив его в папку "Удаленные", делегат должен использовать [операцию MoveItem](moveitem-operation.md). 
  
## <a name="deleteitem-request-example"></a>Пример запроса DeleteItem

### <a name="description"></a>Description

В приведенном ниже примере запроса **DeleteItem** показано, как выполнить окончательное удаление элемента из почтового ящика. 
  
> [!NOTE]
> Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteItem DeleteType="HardDelete" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemIds>
        <t:ItemId Id="AS4AUn=="/>
      </ItemIds>
    </DeleteItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [DeleteItem](deleteitem.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
Чтобы найти другие параметры сообщения Request операции **DeleteItem** , изучите иерархию схемы. Начните с элемента [DeleteItem](deleteitem.md) . 
  
## <a name="successful-deleteitem-response"></a>Успешный ответ DeleteItem

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **DeleteItem** . 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [делетеитемреспонсе](deleteitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [делетеитемреспонсемессаже](deleteitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
Чтобы найти другие параметры для ответного сообщения операции **DeleteItem** , изучите иерархию схемы. Начните с элемента [делетеитемреспонсе](deleteitemresponse.md) . 
  
## <a name="deleteitem-error-response"></a>Ответ об ошибке DeleteItem

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса **DeleteItem** . Ошибка была создана, так как Операция попыталась удалить элемент, который не был найден в хранилище Exchange. 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [делетеитемреспонсе](deleteitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [делетеитемреспонсемессаже](deleteitemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
Чтобы найти другие параметры сообщения об ошибке при выполнении операции **DeleteItem** , изучите иерархию схемы. Начните с элемента [делетеитемреспонсе](deleteitemresponse.md) . 
  
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Удаление контактов](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)  
- [Удаление сообщений электронной почты](https://msdn.microsoft.com/library/c40f2f0b-dae0-412f-b716-727e8c0949b4%28Office.15%29.aspx) 
- [Удаление задач](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

