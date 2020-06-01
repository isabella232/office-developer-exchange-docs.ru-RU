---
title: ункновнентриес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnknownEntries
api_type:
- schema
ms.assetid: 107ec73e-083a-4956-9d37-33d4734cc157
description: Элемент Ункновнентриес содержит массив неизвестных записей разрешений, которые не удается разрешить в службе каталогов Active Directory. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 68cb2518b895ca0a74e6b9ed649ee92b7502ab05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459421"
---
# <a name="unknownentries"></a>ункновнентриес

Элемент **ункновнентриес** содержит массив неизвестных записей разрешений, которые не удается разрешить в службе каталогов Active Directory. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<UnknownEntries>
   <UnknownEntry/>
</UnknownEntries>
```

 **аррайофункновнентриестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ункновнентри](unknownentry.md) <br/> |Представляет одну неизвестную запись разрешения, которая не может быть разрешена в Active Directory. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PermissionSet (Пермиссионсеттипе)](permissionset-permissionsettype.md) <br/> |Содержит все разрешения, настроенные для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[PermissionSet (Календарпермиссионсеттипе)](permissionset-calendarpermissionsettype.md) <br/> |Содержит все разрешения, настроенные для папки календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Примечания

Вы можете удалять неизвестные записи из папки с помощью операции операцию UpdateFolder с элементом [сетфолдерфиелд](setfolderfield.md) . Неизвестные записи удаляются при сбросе набора разрешений с помощью параметра Сетфолдерфиелд операции операцию UpdateFolder. Веб-службы Exchange не поддерживают удаление отдельных записей. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateFolder](updatefolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

