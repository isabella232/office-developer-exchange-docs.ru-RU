---
title: плайонфонинаблед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneEnabled
api_type:
- schema
ms.assetid: 6f800912-be4c-46f9-aa1e-dff0bbf877c5
description: Элемент Плайонфонинаблед указывает, включена ли функция проигрывания на телефоне.
ms.openlocfilehash: 8342e2bcc9c767903e0f6c180000a0f00eccc311
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529933"
---
# <a name="playonphoneenabled"></a>плайонфонинаблед

Элемент **плайонфонинаблед** указывает, включена ли функция проигрывания на телефоне. 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
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
|[унифиедмессагингконфигуратион](unifiedmessagingconfiguration.md) <br/> |Содержит сведения о конфигурации для службы единой системы обмена сообщениями.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент **плайонфонинаблед** имеет значение **true** , если для учетной записи включено воспроизводимое по телефону; в противном случае — значение **false**.
  
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

