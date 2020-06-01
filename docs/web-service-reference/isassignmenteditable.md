---
title: исассигнментедитабле
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsAssignmentEditable
api_type:
- schema
ms.assetid: 0ddf9181-f65e-4ad6-ad69-7b074ea0f2e7
description: Элемент Исассигнментедитабле представляет тип задачи.
ms.openlocfilehash: 5eb091b24e2c97f7aa6072044fed998b6c9c1651
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468056"
---
# <a name="isassignmenteditable"></a>исассигнментедитабле

Элемент **исассигнментедитабле** представляет тип задачи. 
  
```xml
<IsAssignmentEditable/>
```

 **положительн**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Это свойство доступно только для чтения. В приведенной ниже таблице перечислены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|нуль  <br/> |Значение по умолчанию для всех элементов Task.  <br/> |
|1   <br/> |Запрос задачи.  <br/> |
|2  <br/> |Принятие задачи от получателя запроса задачи.  <br/> |
|4  <br/> |Отклонение задачи от получателя запроса задачи.  <br/> |
|4   <br/> |Обновление запроса на предыдущую задачу.  <br/> |
|5   <br/> |Не используется.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

