---
title: MaxMessageSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxMessageSize
api_type:
- schema
ms.assetid: bb98ac72-9409-4332-81bb-ee3bebb9a00e
description: Элемент MaxMessageSize представляет максимальный размер сообщения, можно принять получателя.
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834383"
---
# <a name="maxmessagesize"></a>MaxMessageSize

Элемент **MaxMessageSize** представляет максимальный размер сообщения, можно принять получателя. 
  
```XML
<MaxMessageSize/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Почтовые подсказки](mailtips.md) <br/> |Представляет значения для различных типов почтовые подсказки.  <br/> |
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Содержит сведения о конфигурации службы для службы советы почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — целое число, представляющее максимальный размер сообщения получателя может принимать. Это значение может быть измеряемую в килобайт или мегабайт.
  
## <a name="remarks"></a>Замечания

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

