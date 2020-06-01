---
title: аджацентмитингс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdjacentMeetings
api_type:
- schema
ms.assetid: 50a9c381-9166-476e-8421-29e51b94499b
description: Элемент Аджацентмитингс определяет все элементы календаря, смежные с временем собрания.
ms.openlocfilehash: 7c89095e24af799df22a848be06a0fd65d53be7f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463582"
---
# <a name="adjacentmeetings"></a>аджацентмитингс

Элемент **аджацентмитингс** определяет все элементы календаря, смежные с временем собрания. 
  
```xml
<AdjacentMeetings>
   <CalendarItem/>
</AdjacentMeetings>
```

 **нонемптяррайофаллитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
> [!NOTE]
> Несмотря на то что в схеме допустимы дополнительные дочерние элементы, элемент [календаритем](calendaritem.md) является единственным дочерним элементом, который веб-службы Exchange (EWS) будут возвращать в элементе **аджацентмитингс** . В этой статье не перечислены дочерние элементы, допустимые для схемы, но не возвращенные службой EWS. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

