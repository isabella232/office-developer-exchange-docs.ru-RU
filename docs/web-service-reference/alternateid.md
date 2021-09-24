---
title: AlternateId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AlternateId
api_type:
- schema
ms.assetid: 9c01fdc3-4adf-4e23-bc33-45d2a45ea08b
description: Элемент AlternateId описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в ответе.
ms.openlocfilehash: 6346a45b48eb811cac705d8da85dc77e6c18262c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520943"
---
# <a name="alternateid"></a>AlternateId

Элемент **AlternateId** описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в ответе. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **AlternateIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Описывает исходный идентификатор в запросе [операции ConvertId](convertid-operation.md) и описывает идентификатор назначения в ответе [операции ConvertId.](convertid-operation.md)  <br/> |
|Формат  <br/> |Описывает исходный формат в запросе [операции ConvertId](convertid-operation.md) и описывает формат назначения в ответе [операции ConvertId.](convertid-operation.md) Формат назначения описывается **атрибутом DestinationFormat** элемента [ConvertId](convertid.md) в запросе. Этот атрибут имеет тип **IdFormatType**.  <br/> |
|Mailbox  <br/> |Описывает основной почтовый ящик Простой протокол передачи почты (SMTP), содержащий идентификаторы для перевода.  <br/> |
|IsArchive  <br/> |Указывает, представляет ли идентификатор архивный элемент или папку. Значение true **указывает,** что идентификатор представляет архивный элемент или папку. Этот атрибут является необязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Значения атрибута формата

|**Значение**|**Описание**|
|:-----|:-----|
|EwsLegacyId  <br/> |Описывает идентификаторы, которые Exchange веб-служб в начальной версии Exchange 2007 г.  <br/> |
|EwsId  <br/> |Описывает идентификаторы, которые Exchange веб-Exchange 2007 года.  <br/> |
|EntryId  <br/> |Описывает идентификаторы MAPI, как в **PR_ENTRYID** свойстве.  <br/> |
|HexEntryId  <br/> |Описывает кодированное с гексадецимальным кодом представление свойства **PR_ENTRYID.** Это формат идентификаторов событий календаря доступности.  <br/> |
|StoreId  <br/> |Описывает Exchange идентификаторы магазина.  <br/> |
|OwaId  <br/> |Описывает идентификатор Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConvertIdResponseMessage](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса [на операцию ConvertId.](convertid-operation.md)  <br/> |
|[SourceIds](sourceids.md) <br/> |Содержит исходные идентификаторы для преобразования.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Элемент **AlternateId** описывает два идентификатора, исходный идентификатор, который должен быть преобразован в запросе на операцию [ConvertId,](convertid-operation.md) и преобразованный идентификатор в [элементе ConvertIdResponse.](convertidresponse.md) 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

||||
|:-----|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

