---
title: конфликтресултс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictResults
api_type:
- schema
ms.assetid: 08cdd547-4de7-4c7a-b60f-e618dc217d20
description: Элемент Конфликтресултс содержит количество конфликтов в ответе операции UpdateItem.
ms.openlocfilehash: 923c7950e21039adf28e232486f4df5fc04889d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460171"
---
# <a name="conflictresults"></a>конфликтресултс

Элемент [конфликтресултс](conflictresults.md) содержит количество конфликтов в ответе [операции UpdateItem](updateitem-operation.md) . 
  
[упдатеитемреспонсе](updateitemresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[упдатеитемреспонсемессаже](updateitemresponsemessage.md)
  
[конфликтресултс](conflictresults.md)
  
```xml
<ConflictResults>
   <Count/>
</ConflictResults>
```

 **конфликтресултстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Count](count.md) <br/> |Содержит количество конфликтов в отклике [операции UpdateItem](updateitem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[упдатеитемреспонсемессаже](updateitemresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции UpdateItem](updateitem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateItem](updateitem-operation.md)
  
 **конфликтресултстипе**

