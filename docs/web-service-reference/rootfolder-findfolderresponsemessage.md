---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: Элемент RootFolder содержит результаты поиска одной корневой папки во время операции FindFolder.
ms.openlocfilehash: 582d4642bb4ecd2816beba6df863eb274762f804
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512277"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

Элемент **RootFolder** содержит результаты поиска одной корневой папки во время операции [FindFolder.](findfolder-operation.md)
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |Представляет следующий индекс, который следует использовать для следующего запроса при использовании проиндексного представления для проиндексации.  <br/> |
|NumeratorOffset  <br/> |Представляет новое значение числитель, используемую для следующего запроса при использовании дробных представлений страниц.  <br/> |
|AbsoluteDenominator  <br/> |Представляет следующий знаменатель, который будет использовать для следующего запроса при дробной прогонах.  <br/> |
|IncludesLastItemInRange  <br/> |Указывает, содержатся ли в текущих результатах последняя папка запроса, что дополнительная раскладка не требуется.  <br/> |
|TotalItemsInView  <br/> |Представляет общее число папок, которые проходят ограничение.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, найденных с помощью операции [FindFolder.](findfolder-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции FindFolder.](findfolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindFolder](findfolder-operation.md)


[Поиск папок](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

