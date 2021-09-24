---
title: Attributions (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: Элемент Attributions указывает массив сведений об атрибуции для одного или более контактов или получателей Active Directory, агрегированных в связанную персону.
ms.openlocfilehash: 2c0ee8100398846be33827b5129557ca89789a17
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522030"
---
# <a name="attributions-arrayofpersonaattributionstype"></a>Attributions (ArrayOfPersonaAttributionsType)

Элемент **Attributions** указывает массив сведений об атрибуции для одного или более контактов или получателей Active Directory, агрегированных в связанную персону. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 **ArrayOfPersonaAttributionsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Attribution (PersonaAttributionType)](attribution-personaattributiontype.md) <br/> |Указывает экземпляр в массиве атрибутов элемента **PersonaType.**  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Роль](persona.md) <br/> |Указывает набор данных persona, возвращаемого по запросу **GetPersona.**  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

