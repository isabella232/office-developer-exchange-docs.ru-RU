---
title: Имена внутренних доменов (Смтпдомаинлист)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: Элемент имена внутренних доменов определяет список внутренних доменов SMTP Организации.
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459968"
---
# <a name="internaldomains-smtpdomainlist"></a>Имена внутренних доменов (Смтпдомаинлист)

Элемент **имена внутренних доменов** определяет список внутренних доменов SMTP Организации. 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 **смтпдомаинлист**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домен](domain.md) <br/> |Определяет один домен SMTP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Маилтипсконфигуратион (Маилтипссервицеконфигуратион)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Содержит сведения о конфигурации службы для советов почтового ящика.  <br/> |
|[протектионрулесконфигуратион](protectionrulesconfiguration.md) <br/> |Содержит сведения о конфигурации службы для службы правил защиты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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

