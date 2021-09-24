---
title: ExcludeConflicts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExcludeConflicts
api_type:
- schema
ms.assetid: ec33ef23-8537-41eb-8d89-7eb906a1fad7
description: Элемент ExcludeConflicts указывает, следует ли возвращать рекомендуемые сроки для календарного времени, которое конфликтуется между участниками.
ms.openlocfilehash: 6182ff8faed62cefc39015d3242bf7e669660b4a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539910"
---
# <a name="excludeconflicts"></a>ExcludeConflicts

Элемент **ExcludeConflicts** указывает, следует ли возвращать рекомендуемые сроки для календарного времени, которое конфликтуется между участниками. 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[MailboxDataArray](mailboxdataarray.md)
  
[MailboxData](mailboxdata.md)
  
[ExcludeConflicts](excludeconflicts.md)
  
```xml
<ExcludeConflicts>true or false</ExcludeConflicts>
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
|[MailboxData](mailboxdata.md) <br/> |Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.  <br/> XPath для этого элемента:  <br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Возможные значения — значение Boolean **true или** **false.**
  
## <a name="remarks"></a>Заметки

Этот элемент обязательный.
  
> [!NOTE]
> Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)


[Getting User Availability](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

