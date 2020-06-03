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
description: Элемент BodyType определяет способ форматирования основного текста в отклике.
ms.openlocfilehash: 448d20ac54b09a2f4f6a273a1099519371ac7f5b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465949"
---
# <a name="bodytype"></a>BodyType

Элемент **BodyType** определяет способ форматирования основного текста в отклике. 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

**бодитипереспонсетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемшапе](itemshape.md) <br/> | Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.  <br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[аттачментшапе](attachmentshape.md) <br/> |Определяет дополнительные свойства расширенного элемента, которые возвращаются в ответ на запрос [GetAttachment](getattachment.md) .  <br/><br/>Ниже приведено выражение XPath для этого элемента:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **BodyType** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Лучший  <br/> |Ответ будет возвращать наиболее широко доступное содержимое основного текста. Это полезно, если он неизвестен, является ли контент текстовым или HTML-кодом.<br/><br/> Возвращаемый текст будет содержать текст, если сохраненный текст является обычным текстом. В противном случае ответ вернет HTML, если сохраненный текст имеет формат HTML или RTF.<br/><br/> Это значение используется по умолчанию.  <br/> |
|HTML  <br/> |Ответ вернет основной текст элемента в виде HTML-кода.  <br/> |
|Текст  <br/> |Ответ вернет текст элемента в виде обычного текста.  <br/> |
   
## <a name="remarks"></a>Примечания

Вы можете определить тип текста, возвращаемого в ответе, проверив атрибут **BodyType** элемента [Body](body.md) . Атрибут **BodyType** будет определять основной текст как HTML или как текст. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере запроса показано, где используется элемент **BodyType** . 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Атрибут ID был укорочен для сохранения удобочитаемости.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

