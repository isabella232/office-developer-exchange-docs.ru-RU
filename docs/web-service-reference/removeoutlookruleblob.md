---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: Элемент RemoveOutlookRuleBlob указывает, следует ли удалять blob Outlook правила Майкрософт.
ms.openlocfilehash: 92fd4e22ce0551c7922036e68fc0c6822a006b89
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525598"
---
# <a name="removeoutlookruleblob"></a>RemoveOutlookRuleBlob

Элемент **RemoveOutlookRuleBlob** указывает, следует ли удалять blob Outlook microsoft. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[RemoveOutlookRuleBlob](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
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
|[UpdateInboxRules](updateinboxrules.md) <br/> |Определяет запрос на обновление правил "Входящие" в почтовом ящике в серверном магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текстового **значения true** указывает на то, что Outlook blob правила следует удалить. Ложное **текстовое** значение указывает на то, что Outlook blob правила не следует удалять. 
  
## <a name="remarks"></a>Заметки

Установите этот элемент **true,** чтобы разрешить обновление правила "Входящие". 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateInboxRules](updateinboxrules-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

