---
title: исреадрецеипт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: Элемент Исреадрецеипт указывает, должны ли входящие сообщения принимать уведомления о прочтении для того, чтобы условие или исключение применялось.
ms.openlocfilehash: e86a7776bc43204dae9fc92f21d4304255ddb888
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463904"
---
# <a name="isreadreceipt"></a>исреадрецеипт

Элемент **исреадрецеипт** указывает, должны ли входящие сообщения принимать уведомления о прочтении для того, чтобы условие или исключение применялось. 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
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
|[Условия](conditions.md) <br/> |Представляет условия, если выполнены, запустит действия правил для этого правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет доступных исключение условий для правила папки «Входящие».  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что сообщение должно быть уведомлением о прочтении, чтобы применялось условие или исключение. Если сообщение не обязательно должно быть уведомлением о прочтении для условия или исключения, значение равно **false**.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

