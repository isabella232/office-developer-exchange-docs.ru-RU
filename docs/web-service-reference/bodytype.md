---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: Элемент BodyType определяет способ форматирования основного текста в ответе.
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761595"
---
# <a name="bodytype"></a>BodyType

Элемент **BodyType** определяет способ форматирования основного текста в ответе. 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**BodyTypeResponseType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> | Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.  <br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Определяет дополнительные расширенные свойства элемента для возврата в ответ на запрос [GetAttachment](getattachment.md) .  <br/><br/>Ниже приведен выражение XPath для этого элемента.<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **типа текста сообщения** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Рекомендации  <br/> |В ответе будут возвращены содержательности доступное содержимое основного текста. Это полезно, если не известно, является ли содержимое текста или HTML.<br/><br/> Возвращаемое значение body будет текст основному сохраненных обычного текста. В противном случае ответ вернет HTML Если сохраненные текст в формате HTML или RTF.<br/><br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |Основной текст элемента возвращает ответ как HTML.  <br/> |
|Text  <br/> |В ответе будут возвращены основной текст элемента, как обычный текст.  <br/> |
   
## <a name="remarks"></a>Замечания

Можно определить тип возвращаемого в ответе, установив атрибут **BodyType** элемента [Body](body.md) текст. Атрибут **BodyType** определяет текст HTML или текст. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Следующий пример запроса показано, где используется элемент **типа текста сообщения** . 
  
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
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

В атрибуте Id был усечен, чтобы сохранить удобочитаемость.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

