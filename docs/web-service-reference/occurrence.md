---
title: Экземпляр
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: Элемент вхождения представляет один измененный экземпляр повторяющегося элемента календаря.
ms.openlocfilehash: c3a6bcce23f0bb1125dbd2a5bb86e9b20039a4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466320"
---
# <a name="occurrence"></a>Экземпляр

Элемент **вхождения** представляет один измененный экземпляр повторяющегося элемента календаря. 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

**оккурренцеинфотипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и изменяет ключ измененного экземпляра повторяющегося элемента календаря.  <br/> |
|[Начало](start.md) <br/> |Представляет время начала измененного экземпляра повторяющегося элемента календаря.  <br/> |
|[Оканчиваться](end-ex15websvcsotherref.md) <br/> |Представляет время окончания измененного экземпляра повторяющегося элемента календаря.  <br/> |
|[оригиналстарт](originalstart.md) <br/> |Представляет исходное время начала измененного экземпляра повторяющегося элемента календаря.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[модифиедоккурренцес](modifiedoccurrences.md) <br/> |Содержит коллекцию повторяющихся экземпляров повторяющихся элементов календаря, которые были изменены таким образом, что они отличаются от элемента шаблона повторения.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

