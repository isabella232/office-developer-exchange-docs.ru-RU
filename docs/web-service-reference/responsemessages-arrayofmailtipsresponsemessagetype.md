---
title: Респонсемессажес (Аррайофмаилтипсреспонсемессажетипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: 00878187-fac2-45b9-ba1c-df7ffac71089
description: Элемент Респонсемессажес представляет список ответных сообщений с советами по почте.
ms.openlocfilehash: 2db58029ead9332b832006bc81d751d77df54b07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465452"
---
# <a name="responsemessages-arrayofmailtipsresponsemessagetype"></a>Респонсемессажес (Аррайофмаилтипсреспонсемессажетипе)

Элемент **респонсемессажес** представляет список ответных сообщений с советами по почте. 
  
```XML
<ResponseMessages>
   <MailTipsResponseMessageType/>
</ResponseMessages>
```

 **аррайофмаилтипсреспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[маилтипсреспонсемессажетипе](mailtipsresponsemessagetype.md) <br/> |Представляет параметры почтовых подсказок.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетмаилтипсреспонсе](getmailtipsresponse.md) <br/> |Представляет ответное сообщение для операции с помощью [подсказки](getmailtips-operation.md).  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
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



[Операция GetMailTips](getmailtips-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

