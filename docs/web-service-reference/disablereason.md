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
ms.openlocfilehash: f900bd1b98b294900f767c778b9c5f87f74042ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762127"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

