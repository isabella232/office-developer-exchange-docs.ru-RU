---
title: ImAddresses3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cab51a28-dfad-4c70-aafe-e239321b784e
description: Элемент ImAddresses3 указывает массив адресов мгновенных сообщений и идентификаторы их исходных атрибутов для связанной персоны.
ms.openlocfilehash: 9a3106c0d3f51d090acaf0e23ffb817cb48fc8ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541156"
---
# <a name="imaddresses3"></a>ImAddresses3

Элемент **ImAddresses3 указывает** массив адресов мгновенных сообщений и идентификаторы их исходных атрибутов для связанной персоны. 
  
```XML
<ImAddresses3>
    <StringAttributedValue/>
</ImAddresses3>
```

 **ArrayOfStringAttributedValuesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StringAttributedValue](stringattributedvalue.md) <br/> |Указывает экземпляр в массиве атрибутов, связанных с элементом persona.  <br/> |
   
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

