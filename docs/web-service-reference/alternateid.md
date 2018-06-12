---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: Элемент AlternateId описание идентификатора для преобразования в запрос и результаты преобразованных идентификатор в ответе.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761370"
---
# <a name="alternateid"></a>AlternateId

Элемент **AlternateId** описание идентификатора для преобразования в запрос и результаты преобразованных идентификатор в ответе. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Описывает идентификатор источника в запрос [операции ConvertId](convertid-operation.md) и идентификатор назначения в [операцию ConvertId](convertid-operation.md) ответа.  <br/> |
|Формат  <br/> |Описывает формат источника в запрос [операции ConvertId](convertid-operation.md) и формат назначения в [операцию ConvertId](convertid-operation.md) ответа. Формат назначения описывается атрибут **DestinationFormat** элемента [ConvertId](convertid.md) в запросе. Этот атрибут имеет тип **IdFormatType**.  <br/> |
|Почтовый ящик  <br/> |Описывает почтового ящика основной Simple Mail Transfer Protocol (SMTP) адрес, содержащий идентификаторы для перевода.  <br/> |
|IsArchive  <br/> |Указывает, представляет ли идентификатор архивных элемента или папки. Значение **true** указывает, что идентификатор представляет архивных элемента или папки. Этот атрибут является необязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Значения атрибутов формата

|**Значение**|**Описание**|
|:-----|:-----|
|EwsLegacyId  <br/> |Описываются идентификаторы, которые создаются веб-служб Exchange в первоначальной версии Exchange 2007.  <br/> |
|EwsId  <br/> |Описываются идентификаторы, которые создаются веб-служб Exchange, начиная с Exchange 2007 с пакетом обновления 1.  <br/> |
|Идентификатор записи  <br/> |Описываются идентификаторы MAPI, как и свойство **PR_ENTRYID** .  <br/> |
|HexEntryId  <br/> |Описывает представление шестнадцатеричном формате **PR_ENTRYID** свойства. Это формат идентификаторы событий календаря доступности.  <br/> |
|StoreId  <br/> |Описываются идентификаторы хранилища Exchange.  <br/> |
|OwaId  <br/> |Описывает идентификатор Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат [операции ConvertId](convertid-operation.md) запроса.  <br/> |
|[SourceIds](sourceids.md) <br/> |Содержит идентификаторы источника для преобразования.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Элемент **AlternateId** описание двух идентификаторов, идентификатор источника, который должен быть преобразован в запрос [операции ConvertId](convertid-operation.md) и преобразованные идентификатор в элементе [ConvertIdResponse](convertidresponse.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

||||
|:-----|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

