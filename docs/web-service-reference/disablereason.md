---
title: дисаблереасон
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f41b5be6-9b79-4e83-8cdb-aa779e13cb3f
description: Элемент Дисаблереасон указывает причину отключения приложения.
ms.openlocfilehash: 1406d69647bde5389dc9bb61adf7537a57d5adfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463673"
---
# <a name="disablereason"></a>дисаблереасон

Элемент **дисаблереасон** указывает причину отключения приложения. 
  
```XML
<DisableReason> NoReason | OutlookClientPerformance | OWAClientPerformance | MobileClientPerformance </DisableReason>
```

 **дисаблереасонтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DisableApp](disableapp.md) <br/> |Указывает запрос на отключение приложения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**Текстовое значение элемента Дисаблереасон**

|**Значение**|**Описание**|
|:-----|:-----|
|Причина  <br/> |Причина не задана  <br/> |
|аутлукклиентперформанце  <br/> |Для повышения производительности почтового клиента.  <br/> |
|оваклиентперформанце  <br/> |Для повышения производительности клиента веб-приложения.  <br/> |
|мобилеклиентперформанце  <br/> |Для повышения производительности мобильных клиентов.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

