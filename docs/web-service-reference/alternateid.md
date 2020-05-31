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
description: Элемент AlternateId описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в отклике.
ms.openlocfilehash: e4d29087b63b52638dd93e4e3b643cdee39a5b97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761370"
---
# <a name="alternateid"></a>AlternateId

Элемент **AlternateId** описывает идентификатор для преобразования в запросе и результаты преобразованного идентификатора в отклике. 
  
```XML
<AlternateId Id="" Format="" Mailbox="" IsArchive=""/>
```

 **алтернатеидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Описывает идентификатор источника в запросе [операции ConvertId](convertid-operation.md) и описывает идентификатор назначения в ответе [операции ConvertId](convertid-operation.md) .  <br/> |
|Format  <br/> |Описывает исходный формат в запросе [операции ConvertId](convertid-operation.md) и описывает формат назначения в ответе [операции ConvertId](convertid-operation.md) . Формат назначения описывается атрибутом **дестинатионформат** элемента [ConvertId](convertid.md) в запросе. Этот атрибут относится к типу **идформаттипе**.  <br/> |
|Почтовый ящик  <br/> |Описывает основной SMTP-адрес почтового ящика, который содержит идентификаторы для преобразования.  <br/> |
|IsArchive  <br/> |Указывает, представляет ли идентификатор архивированный элемент или папку. Значение **true** указывает, что идентификатор представляет архивный элемент или папку. Этот атрибут является необязательным.  <br/> |
   
#### <a name="format-attribute-values"></a>Форматирование значений атрибутов

|**Значение**|**Описание**|
|:-----|:-----|
|евслегациид  <br/> |Описывает идентификаторы, созданные веб-службами Exchange в исходной версии Exchange 2007.  <br/> |
|евсид  <br/> |Описание идентификаторов, создаваемых веб-службами Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).  <br/> |
|Код  <br/> |Описывает идентификаторы MAPI, как в свойстве **PR_ENTRYID** .  <br/> |
|хексентрид  <br/> |Описывает представление свойства **PR_ENTRYID** в шестнадцатеричном формате. Это формат идентификаторов событий календаря доступности.  <br/> |
|StoreId  <br/> |Описывает идентификаторы хранилища Exchange.  <br/> |
|оваид  <br/> |Описывает идентификатор Outlook Web App.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конвертидреспонсемессаже](convertidresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции ConvertId](convertid-operation.md) .  <br/> |
|[саурцеидс](sourceids.md) <br/> |Содержит идентификаторы источников для преобразования.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Элемент **AlternateId** описывает два идентификатора, идентификатор источника, который необходимо преобразовать в запрос [операции ConvertId](convertid-operation.md) , и преобразованный идентификатор в элементе [конвертидреспонсе](convertidresponse.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

||||
|:-----|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ConvertId](convertid-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Преобразование идентификаторов](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

