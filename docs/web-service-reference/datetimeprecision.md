---
title: датетимепреЦисион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 822dc5a6-2d57-474b-8a7d-da150898e5b6
description: Элемент ДатетимепреЦисион указывает точность возвращаемых значений даты и времени.
ms.openlocfilehash: 9d245dfb0123daae42ba9b9b4e98aff872b67d80
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529226"
---
# <a name="datetimeprecision"></a>датетимепреЦисион

Элемент **датетимепреЦисион** указывает точность возвращаемых значений даты и времени. 
  
```XML
<DateTimePrecision />
```

**датетимепреЦисионтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

Элемент **датетимепреЦисион** находится в заголовке SOAP. 
  
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже перечислены возможные значения.
  
- Секунды
    
- Миллисекундах
    
## <a name="remarks"></a>Примечания

Если используется заголовок SOAP с элементом **датетимепреЦисион** , для которого задано значение "секунды", значения даты и времени возвращаются к ближайшей секунде (00:00:00). При использовании параметра "миллисекунды" значения даты и времени возвращаются до ближайшей миллисекунды (00:00:00.0000). 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   

