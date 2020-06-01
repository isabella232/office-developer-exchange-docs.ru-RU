---
title: Указав
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: Элемент ConfigurationName указывает запрошенные конфигурации службы по имени.
ms.openlocfilehash: 5e1216253a633af643dbd276827842dbe2db5d5f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463925"
---
# <a name="configurationname"></a>Указав

Элемент **configurationName** указывает запрошенные конфигурации службы по имени. 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 **сервицеконфигуратионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[рекуестедконфигуратион](requestedconfiguration.md) <br/> |Содержит требуемые конфигурации службы.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **configurationName** . 
  
**Значения элементов ConfigurationName**

|**Значение**|**Описание**|
|:-----|:-----|
|Подсказки  <br/> |Определяет конфигурацию службы почтовых подсказок.  <br/> |
|унифиедмессагингконфигуратион  <br/> |Определяет конфигурацию службы единой системы обмена сообщениями.  <br/> |
|протектионрулес  <br/> |Определяет конфигурацию службы правил защиты.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

