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
ms.openlocfilehash: 1fd3ceb629689c560dc60afe01f0413602f79a0d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835491"
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

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetMailTips](getmailtips-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

