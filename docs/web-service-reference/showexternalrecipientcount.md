---
title: шовекстерналреЦипиенткаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Элемент ШовекстерналреЦипиенткаунт указывает, должны ли потребители операции с подсказками показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460472"
---
# <a name="showexternalrecipientcount"></a>шовекстерналреЦипиенткаунт

Элемент **шовекстерналреЦипиенткаунт** указывает, должны ли потребители [операции](getmailtips-operation.md) с подсказками показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
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
|[Маилтипсконфигуратион (Маилтипссервицеконфигуратион)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Содержит сведения о конфигурации службы для советов почтового ящика.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение этого элемента имеет значение **true** , если потребители [операции](getmailtips-operation.md) с подсказками должны отображать подсказки для почты, указывающие количество внешних получателей, на которые адресовано сообщение. Значение **false** , если потребители [операции](getmailtips-operation.md) с подсказками не должны показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMailTips](getmailtips-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

