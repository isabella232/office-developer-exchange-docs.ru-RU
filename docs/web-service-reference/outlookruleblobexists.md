---
title: аутлукрулеблобексистс
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
description: Элемент Аутлукрулеблобексистс указывает, существует ли большой двоичный объект правила Microsoft Outlook в почтовом ящике пользователя.
ms.openlocfilehash: 6a5c2a2ec0246d38b22279b86772972ea81922c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529030"
---
# <a name="outlookruleblobexists"></a>аутлукрулеблобексистс

Элемент **аутлукрулеблобексистс** указывает, существует ли большой двоичный объект правила Microsoft Outlook в почтовом ящике пользователя. 
  
[жетинбоксрулесреспонсе](getinboxrulesresponse.md)
  
[аутлукрулеблобексистс](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
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
|[жетинбоксрулесреспонсе](getinboxrulesresponse.md) <br/> |Представляет ответ на запрос [операции GetInboxRules](getinboxrules-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что существует большой двоичный объект правила Outlook. Текстовое значение **false** указывает, что большой двоичный объект правила Outlook не существует. 
  
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

