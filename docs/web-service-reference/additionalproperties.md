---
title: аддитионалпропертиес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: Элемент Аддитионалпропертиес определяет дополнительные свойства для использования в запросах GetItem, UpdateItem, CreateItem, FindItem или FindFolder.
ms.openlocfilehash: 90a307ba4d5ece10e15d2cec56cf5042c3d38685
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455816"
---
# <a name="additionalproperties"></a>аддитионалпропертиес

Элемент **аддитионалпропертиес** определяет дополнительные свойства для использования в запросах [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или [FindFolder](findfolder.md) . 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 **нонемптяррайофпасстоелементтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[екстендедфиелдури](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI, которые необходимо получить, задать или создать.  <br/> |
|[фиелдури](fielduri.md) <br/> |Определяет часто упоминаемые свойства по URI.  <br/> |
|[индекседфиелдури](indexedfielduri.md) <br/> |Определяет свойства часто упоминаемого словаря по универсальному коду ресурса (URI).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдершапе](foldershape.md) <br/> | Определяет свойства папки, включаемые в ответ [на](getfolder.md)SyncFolderHierarchy, [FindFolder](findfolder.md)или [SyncFolderHierarchy](syncfolderhierarchy.md) .<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[итемшапе](itemshape.md) <br/> | Определяет свойства и контент элемента, включаемые в ответ [GetItem](getitem.md), [FindItem](finditem.md)или [SyncFolderItems](syncfolderitems.md) .<br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[аттачментшапе](attachmentshape.md) <br/> |Определяет дополнительные свойства расширенного элемента, которые возвращаются в ответ на запрос [GetItem](getitem.md) .<br/><br/> Ниже приведено выражение XPath для этого элемента:<br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a>Примечания

Не все дочерние элементы могут использоваться с запросами [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или [FindFolder](findfolder.md) . Свойство должно быть применимым к папке или элементу, к которому осуществляется доступ. Используйте расширенные свойства для доступа к другим свойствам. Если свойство не существует для данного элемента, в результирующий XML-файл не будет выдаваться соответствующий элемент. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
Этот элемент является необязательным.
  
## <a name="example"></a>Пример

В приведенном ниже примере запроса показано, как получить тему элемента с помощью элемента **аддитионалпропертиес** . 
  
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
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

