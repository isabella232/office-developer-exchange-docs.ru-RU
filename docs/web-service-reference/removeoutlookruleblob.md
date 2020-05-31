---
title: ремовеаутлукрулеблоб
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: Элемент Ремовеаутлукрулеблоб указывает, следует ли удалить большой двоичный объект правила Microsoft Outlook.
ms.openlocfilehash: 45336e296c39161704ce6e0d51fba1d2c61797b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835102"
---
# <a name="removeoutlookruleblob"></a>ремовеаутлукрулеблоб

Элемент **ремовеаутлукрулеблоб** указывает, следует ли удалить большой двоичный объект правила Microsoft Outlook. 
  
[UpdateInboxRules](updateinboxrules.md)
  
[ремовеаутлукрулеблоб](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
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
|[UpdateInboxRules](updateinboxrules.md) <br/> |Определяет запрос на обновление правил папки "Входящие" в почтовом ящике в хранилище сервера.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение **true** указывает, что большой двоичный объект правила Outlook должен быть удален. Текстовое значение **false** указывает, что большой двоичный объект правила Outlook не должен удаляться. 
  
## <a name="remarks"></a>Примечания

Установите для этого элемента **значение true** , чтобы разрешить обновление правила для папки "Входящие". 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateInboxRules](updateinboxrules-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

