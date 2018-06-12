---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: Элемент IncludeMimeContent указывает, возвращается ли содержимое Multipurpose Internet Mail Extensions (MIME) элемента или вложения в ответе.
ms.openlocfilehash: ddd6988be93231ac7c574a2e19c9ba4b562c7d0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833903"
---
# <a name="includemimecontent"></a>IncludeMimeContent

Элемент **IncludeMimeContent** указывает, возвращается ли содержимое Multipurpose Internet Mail Extensions (MIME) элемента или вложения в ответе. 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | Определяет дополнительные свойства, возвращаемые в ответ на запрос [GetAttachment](getattachment.md) .  <br/> <br/> Ниже приведен выражение XPath для этого элемента.  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.  <br/> <br/> Ниже приведены выражения XPath для этого элемента.<br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Этот элемент может быть значение **true** или **false**. Значение по умолчанию — **false**. Это тип данных Boolean.
  
## <a name="remarks"></a>Замечания

Этот элемент является необязательным.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Запрос в следующем примере показано, как для задания **IncludeMimeContent** элемента. 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

В атрибуте Id вложения усекается, чтобы сохранить удобочитаемость.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

