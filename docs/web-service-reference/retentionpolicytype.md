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
ms.openlocfilehash: 3900718f10e1e11d5864ebf7e64a3e1e22aa45c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462873"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   

