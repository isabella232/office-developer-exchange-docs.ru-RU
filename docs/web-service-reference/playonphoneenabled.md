---
title: PlayOnPhoneEnabled
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
description: Элемент PlayOnPhoneEnabled указывает, включена ли функция воспроизвести на телефоне.
ms.openlocfilehash: 1a6c5c41a4fe723f37d07ad0151dfbd6512cf4f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834829"
---
# <a name="playonphoneenabled"></a>PlayOnPhoneEnabled

Элемент **PlayOnPhoneEnabled** указывает, включена ли функция воспроизвести на телефоне. 
  
```XML
<PlayOnPhoneEnabled>true | false</PlayOnPhoneEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UnifiedMessagingConfiguration](unifiedmessagingconfiguration.md) <br/> |Содержит сведения о конфигурации для службы единой системы обмена сообщениями.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент **PlayOnPhoneEnabled** имеет значение **true** , если этот параметр включен воспроизвести на телефоне для учетной записи; в противном случае — значение **false**.
  
## <a name="remarks"></a>Замечания

Этот элемент обязательный.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

