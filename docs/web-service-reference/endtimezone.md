---
title: EndTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeZone
api_type:
- schema
ms.assetid: 6c53c337-be60-4d22-9e9e-a0c140c5e913
description: Элемент EndTimeZone определяет часовой пояс для времени окончания Календаритем или свойство meetingrequest.
ms.openlocfilehash: 83ab2ab90e2bed7658fe83ed33a72b60d5f10135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462987"
---
# <a name="endtimezone"></a>EndTimeZone

Элемент **EndTimeZone** определяет часовой пояс для времени окончания [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).
  
```xml
<EndTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</EndTimeZone>
```

 **тимезонедефинитионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Представляет уникальный идентификатор определения часового пояса.  <br/> |
|Имя  <br/> |Представляет описательное имя определения часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Periods](periods.md) <br/> |Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.  <br/> |
|[транситионсграупс](transitionsgroups.md) <br/> |Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.  <br/> |
|[Выполняет](transitions.md) <br/> |Представляет массив переходов часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

