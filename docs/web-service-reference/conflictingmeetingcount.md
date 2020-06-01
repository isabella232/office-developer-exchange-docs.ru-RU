---
title: конфликтингмитингкаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConflictingMeetingCount
api_type:
- schema
ms.assetid: 11f4d93a-b514-4a27-8d19-f4f0a35a185e
description: Элемент Конфликтингмитингкаунт представляет количество собраний, которые конфликтуют с элементом календаря.
ms.openlocfilehash: d53245e1b5d1f0182b28b15bf55ba9742bbb2a07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463862"
---
# <a name="conflictingmeetingcount"></a>конфликтингмитингкаунт

Элемент **конфликтингмитингкаунт** представляет количество собраний, которые конфликтуют с элементом календаря. 
  
```xml
<ConflictingMeetingCount/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет целое число. Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Примечания

Элемент календаря считается конфликтующим, если он происходит, по крайней мере, частично, в то же время, что и другой элемент календаря в той же папке "Календарь". Если элемент календаря находится в папке "некалендарный", он сравнивается с элементами календаря в папке "Календарь" по умолчанию. Приглашения на собрания сравниваются с элементами календаря в папке "Календарь" по умолчанию.
  
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

