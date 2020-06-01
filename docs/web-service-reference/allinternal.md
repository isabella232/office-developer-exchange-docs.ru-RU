---
title: аллинтернал
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllInternal
api_type:
- schema
ms.assetid: b7e5072f-5d9f-4ee0-b58b-4d75d878ea1c
description: Элемент Аллинтернал имеет значение true, если все получатели сообщения электронной почты являются внутренними для организации отправителя.
ms.openlocfilehash: c5ffe15eca5d680994acb62913ebf5effacce214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464835"
---
# <a name="allinternal"></a>аллинтернал

Элемент **аллинтернал** имеет **значение true** , если все получатели сообщения электронной почты являются внутренними для организации отправителя. 
  
```xml
<AllInternal/>
```

 **протектионрулеаллинтерналтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Условие](condition.md) <br/> |Определяет условие, которое должно быть удовлетворено для части действия правила, которое необходимо выполнить.  <br/> |
|[И (Протектионрулеандтипе)](and-protectionruleandtype.md) <br/> |Указывает, что все дочерние элементы должны сопоставляться со значением **true**.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент **аллинтернал** должен быть пустым. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

