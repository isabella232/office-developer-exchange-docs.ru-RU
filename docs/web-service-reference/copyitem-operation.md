---
title: CopyItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: Операция CopyItem копирует элементы и размещает элементы в другую папку.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761841"
---
# <a name="copyitem-operation"></a>CopyItem Operation

Операция **CopyItem** копирует элементы и размещает элементы в другую папку. 
  
## <a name="copyitem-request-example"></a>Пример запроса CopyItem

### <a name="description"></a>Описание

В следующем примере запрос **CopyItem** показано, как для формирования запроса скопировать элемент в папке "Входящие". 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

> [!NOTE]
> Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [CopyItem](copyitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [Что ItemID](itemids.md)
    
- [Идентификатор элемента](itemid.md)
    
> [!NOTE]
> Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа. 
  
Чтобы найти другие параметры для запроса операции **CopyItem** , изучите иерархия схемы. Начать с [CopyItem](copyitem.md) элемента. 
  
## <a name="successful-copyitem-response"></a>Успешного ответа CopyItem

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **CopyItem** . 
  
Идентификатор нового элемента, возвращается в сообщении ответа. Идентификаторы элементов не возвращаются в ответ для нескольких почтовых или почтовых ящиков операциям **CopyItem** общей папки. 
  
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
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Элементы](items.md)
    
Чтобы найти другие параметры в сообщении ответа операции **CopyItem** , изучите иерархия схемы. Запустите в элементе [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="copyitem-error-response"></a>Отклик CopyItem

### <a name="description"></a>Описание

В следующем примере показано возврату ошибки **CopyItem** запрос. 
  
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
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Элементы](items.md)
    
Чтобы найти другие параметры в сообщении об ошибке ответа операции **CopyItem** , изучите иерархия схемы. Запустите в элементе [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

