---
title: Рутфолдер (Финдфолдерреспонсемессаже)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: Элемент Рутфолдер содержит результаты поиска в одной корневой папке во время операции FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835253"
---
# <a name="rootfolder-findfolderresponsemessage"></a>Рутфолдер (Финдфолдерреспонсемессаже)

Элемент **рутфолдер** содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **финдфолдерпаренттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|индекседпагингоффсет  <br/> |Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения по страницам.  <br/> |
|нумератороффсет  <br/> |Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений дробной страницы.  <br/> |
|абсолутеденоминатор  <br/> |Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.  <br/> |
|инклудесластитеминранже  <br/> |Указывает, содержит ли текущие результаты последнюю папку в запросе, что не требуется для дальнейшей разбиения на страницы.  <br/> |
|тоталитемсинвиев  <br/> |Представляет общее число папок, которые прошли ограничение.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, найденных с помощью [операции FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[финдфолдерреспонсемессаже](findfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции FindFolder](findfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

