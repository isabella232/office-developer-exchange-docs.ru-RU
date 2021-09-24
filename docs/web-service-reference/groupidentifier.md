---
title: GroupIdentifier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GroupIdentifier
api_type:
- schema
ms.assetid: bdc6fc1e-4979-42da-a35b-e3017988c7d3
description: Элемент GroupIdentifier представляет единый идентификатор безопасности и атрибут для объектной группы объектов службы каталогов Active Directory, членом которой является учетная запись.
ms.openlocfilehash: c96d0ca673d9b488266f08abbbd6546aaeb9f5a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533161"
---
# <a name="groupidentifier"></a>GroupIdentifier

Элемент **GroupIdentifier** представляет единый идентификатор безопасности и атрибут для объектной группы объектов службы каталогов Active Directory, членом которой является учетная запись. 
  
```xml
<GroupIdentifier>
   <SecurityIdentifier/>
</GroupIdentifier>
```

 **SidAndAttributesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Attributes** <br/> |Содержит атрибуты группы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SecurityIdentifier](securityidentifier.md) <br/> |Представляет язык определения дескриптора безопасности (SDDL) формы идентификатора безопасности[(SID),](sid.md)представляют группу.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GroupSids](groupsids.md) <br/> |Представляет коллекцию идентификаторов объектов безопасности объектов группы Active Directory, которые составляют маркер учетной записи для сериализации маркеров. Сериализация маркеров не поддерживается.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

