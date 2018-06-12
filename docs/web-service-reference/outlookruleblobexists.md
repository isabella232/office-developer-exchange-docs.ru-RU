---
title: OutlookRuleBlobExists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: Элемент OutlookRuleBlobExists показывает, существует ли правило большого двоичного объекта Microsoft Outlook в почтовом ящике пользователя.
ms.openlocfilehash: a738377cd3c1d69b90ac39ca479b03b3220d5bc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834679"
---
# <a name="outlookruleblobexists"></a>OutlookRuleBlobExists

Элемент **OutlookRuleBlobExists** показывает, существует ли правило большого двоичного объекта Microsoft Outlook в почтовом ящике пользователя. 
  
[GetInboxRulesResponse](getinboxrulesresponse.md)
  
[OutlookRuleBlobExists](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
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
|[GetInboxRulesResponse](getinboxrulesresponse.md) <br/> |Представляет ответ на запрос [GetInboxRules операции](getinboxrules-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true,** указывает, что существует большой двоичный объект правила Outlook. Текстовое значение **false** указывает, что большой двоичный объект правила Outlook не существует. 
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

