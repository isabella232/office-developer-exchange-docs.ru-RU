---
title: календарфолдерпермиссионлевел
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarFolderPermissionLevel
api_type:
- schema
ms.assetid: 2a5c9381-dc2c-4fc6-b9b5-893477d0970e
description: Элемент Календарфолдерпермиссионлевел содержит разрешения для папки календаря по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: dcbd57da42b5e701d898c3756ce9bcc100c20af7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461466"
---
# <a name="calendarfolderpermissionlevel"></a>календарфолдерпермиссионлевел

Элемент **календарфолдерпермиссионлевел** содержит разрешения для папки календаря по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<CalendarFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</CalendarFolderPermissionLevel>
```

 **делегатефолдерпермиссионлевелтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[делегатепермиссионс](delegatepermissions.md) <br/> |Содержит параметры уровня разрешений Delegate для пользователя. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены текстовые значения, представляющие уровни разрешений.
  
**Текстовые значения уровня разрешений**

|**Уровень разрешений**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Представитель пользователя не имеет разрешений на доступ к папке "Календарь".  <br/> |
|Reviewer  <br/> |Делегированный пользователь может читать элементы в папке "Календарь".  <br/> |
|Автор  <br/> |Делегированный пользователь может читать и создавать элементы в папке "Календарь".  <br/> |
|Корректор  <br/> |Делегированный пользователь может читать, создавать и изменять элементы в папке "Календарь".  <br/> |
|Пользовательские  <br/> |Представитель пользователя имеет пользовательские разрешения на доступ к папке "Календарь".  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

