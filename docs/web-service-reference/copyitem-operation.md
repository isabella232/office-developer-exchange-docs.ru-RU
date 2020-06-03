---
title: Операция CopyItem
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
description: Операция CopyItem копирует элементы и размещает их в другой папке.
ms.openlocfilehash: ec07700a5ebbdc8774aa2134919634b8dfd02406
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462180"
---
# <a name="copyitem-operation"></a>Операция CopyItem

Операция **CopyItem** копирует элементы и размещает их в другой папке. 
  
## <a name="copyitem-request-example"></a>Пример запроса CopyItem

### <a name="description"></a>Description

В приведенном ниже примере запроса **CopyItem** показано, как сформировать запрос на копирование элемента в папку "Входящие". 
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CopyItem](copyitem.md)
    
- [тофолдерид](tofolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
> [!NOTE]
> Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа. 
  
Чтобы найти другие параметры сообщения Request операции **CopyItem** , изучите иерархию схемы. Начните с элемента [CopyItem](copyitem.md) . 
  
## <a name="successful-copyitem-response"></a>Успешный ответ CopyItem

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос **CopyItem** . 
  
В ответном сообщении возвращается идентификатор элемента нового элемента. Идентификаторы элементов не возвращаются в ответах на операции **CopyItem** для нескольких почтовых ящиков или почтовых ящиков в общедоступных папках. 
  
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
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [копитемреспонсе](copyitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [копитемреспонсемессаже](copyitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
Чтобы найти другие параметры для ответного сообщения операции **CopyItem** , изучите иерархию схемы. Начните с элемента [копитемреспонсе](copyitemresponse.md) . 
  
## <a name="copyitem-error-response"></a>Ответ об ошибке CopyItem

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса **CopyItem** . 
  
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
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [копитемреспонсе](copyitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [копитемреспонсемессаже](copyitemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Items](items.md)
    
Чтобы найти другие параметры сообщения об ошибке при выполнении операции **CopyItem** , изучите иерархию схемы. Начните с элемента [копитемреспонсе](copyitemresponse.md) . 
  
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

