---
title: Группы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Groups
api_type:
- schema
ms.assetid: 6b6b2d67-219d-4dfb-a4ed-d627b1cfb33f
description: Элемент Groups содержит коллекцию групп, которые обнаружены с помощью критериев поиска и объединения, которые определены в запросе операции FindItem.
ms.openlocfilehash: 915d9dffd6d8cec1def6634e6b70642d563b5242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530791"
---
# <a name="groups"></a>Группы

Элемент **Groups** содержит коллекцию групп, которые обнаружены с помощью критериев поиска и объединения, которые определены в запросе [операции FindItem](finditem-operation.md) . 
  
```xml
<Groups>
   <GroupedItems/>
</Groups>
```

 **аррайофграупедитемстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[граупедитемс](groupeditems.md) <br/> |Представляет коллекцию элементов, которая является результатом сгруппированного вызова [операции FindItem](finditem-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Рутфолдер (Финдитемреспонсемессаже)](rootfolder-finditemresponsemessage.md) <br/> |Содержит результаты поиска в одной корневой папке во время операции [FindItem](finditem-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Один экземпляр [граупедитемс](groupeditems.md) будет выполняться для каждой отдельной группы в результате. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindItem](finditem-operation.md)


[Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

