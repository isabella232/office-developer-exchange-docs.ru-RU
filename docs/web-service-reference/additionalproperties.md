---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: Элемент AdditionalProperties определяет дополнительные свойства для использования в запросах GetItem, UpdateItem, CreateItem, FindItem или FindFolder.
ms.openlocfilehash: 9a6fb98e9a88b1e40bd83559b1836d4122f0f125
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522203"
---
# <a name="additionalproperties"></a>AdditionalProperties

Элемент **AdditionalProperties** определяет дополнительные свойства для использования в [запросах GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)или [FindFolder.](findfolder.md) 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **NonEmptyArrayOfPathsToElementType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI для получения, набора или создания.  <br/> |
|[FieldURI](fielduri.md) <br/> |Определяет часто ссылаясь свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Определяет часто ссылаясь свойства словаря URI.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Определяет свойства папок, которые необходимо включить в [ответ GetFolder,](getfolder.md) [FindFolder](findfolder.md)или [SyncFolderHierarchy.](syncfolderhierarchy.md)<br/><br/>  Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Определяет свойства и содержимое элемента, которые необходимо включить в [ответ GetItem,](getitem.md) [FindItem](finditem.md)или [SyncFolderItems.](syncfolderitems.md)<br/><br/>  Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[AttachmentShape](attachmentshape.md) <br/> |Определяет дополнительные свойства расширенных элементов, чтобы вернуться в ответ на [запрос GetItem.](getitem.md)<br/><br/> Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>Заметки

Не все детские элементы можно использовать с [запросами GetItem,](getitem.md) [UpdateItem,](updateitem.md) [CreateItem,](createitem.md) [FindItem](finditem.md)или [FindFolder.](findfolder.md) Свойство должно быть применимо к папке или элементу, к нему можно получить доступ. Используйте расширенные свойства для доступа к другим свойствам. Если свойство не существует для данного элемента, соответствующий элемент не будет излучаться в результате XML. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
Этот элемент является необязательным.
  
## <a name="example"></a>Пример

В следующем примере запроса показано, как получить объект с помощью элемента **AdditionalProperties.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

