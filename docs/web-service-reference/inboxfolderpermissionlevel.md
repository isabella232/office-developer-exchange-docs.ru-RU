---
title: инбоксфолдерпермиссионлевел
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InboxFolderPermissionLevel
api_type:
- schema
ms.assetid: f250d31b-9193-4c1c-8350-900dead3a023
description: Элемент Инбоксфолдерпермиссионлевел содержит разрешения для папки "Входящие", используемой по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 8a497a38a58e6455f2bd754aa8da97b421a2bca3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465711"
---
# <a name="inboxfolderpermissionlevel"></a>инбоксфолдерпермиссионлевел

Элемент **инбоксфолдерпермиссионлевел** содержит разрешения для папки "Входящие", используемой по умолчанию. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<InboxFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</InboxFolderPermissionLevel>
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
|Нет  <br/> |Представитель пользователя не имеет разрешений на доступ к папке "Входящие".  <br/> |
|Reviewer  <br/> |Делегированный пользователь может читать элементы в папке "Входящие".  <br/> |
|Автор  <br/> |Делегированный пользователь может читать и создавать элементы в папке "Входящие".  <br/> |
|Корректор  <br/> |Делегированный пользователь может читать, создавать и изменять элементы в папке "Входящие".  <br/> |
|Пользовательские  <br/> |Представитель пользователя имеет пользовательские разрешения на доступ к папке "Входящие".  <br/> |
   
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

