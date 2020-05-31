---
title: ретентионполицитипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: Элемент Ретентионполицитипе указывает тип политики хранения, применяемый к элементам в беседе.
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835229"
---
# <a name="retentionpolicytype"></a>ретентионполицитипе

Элемент **ретентионполицитипе** указывает тип политики хранения, применяемый к элементам в беседе. 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 **RetentionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[конверсатионактион](conversationaction.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **ретентионполицитипе** — это тип хранения, применяемый к элементам в беседе. Текстовое значение **Delete** указывает на то, что элементы беседы удаляются по истечении срока хранения. Текстовое значение **архива** указывает на то, что элементы беседы перемещаются в архивный почтовый ящик при истечении срока хранения. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

