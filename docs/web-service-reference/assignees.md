---
title: Assignees
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: Элемент Assignees указывает людей, которым назначена задача.
ms.openlocfilehash: 1b5368dbe478e51a23f1f0761635e017b935911d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525192"
---
# <a name="assignees"></a>Assignees

Элемент **Assignees** указывает людей, которым назначена задача. 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 **EmailUserType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Name (EmailAddress)](name-emailaddress.md) <br/> |Отображает имя пользователя почтового ящика.  <br/> |
|[UserId (строка)](userid-string.md) <br/> |Указывает идентификатор пользователя пользователя электронной почты.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TaskSuggestion](tasksuggestion.md) <br/> |Указывает предложенную задачу.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

