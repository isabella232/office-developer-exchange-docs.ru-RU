---
title: уменаблед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UmEnabled
api_type:
- schema
ms.assetid: 87382d9b-0c02-49ec-85dc-3f5918df3195
description: Элемент Уменаблед указывает, включена ли единая система обмена сообщениями для учетной записи.
ms.openlocfilehash: 7ba7be69868cb439177702f74ff4a2f12875b7ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468357"
---
# <a name="umenabled"></a>уменаблед

Элемент **уменаблед** указывает, включена ли единая система обмена сообщениями для учетной записи. 
  
```XML
<UmEnabled>true | false</UmEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[унифиедмессагингконфигуратион](unifiedmessagingconfiguration.md) <br/> |Содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **уменаблед** имеет **значение true** , если для учетной записи включена единая система обмена сообщениями; в противном случае — значение **false**.
  
## <a name="remarks"></a>Примечания

Этот элемент обязательный.
  
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

