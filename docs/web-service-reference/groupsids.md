---
title: GroupSids
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupSids
api_type:
- schema
ms.assetid: ebb00653-83f0-4080-a902-c38df6719800
description: Элемент GroupSids представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.
ms.openlocfilehash: c24c8ea3c3b7d37f41986997ed924c951b4a48ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833790"
---
# <a name="groupsids"></a>GroupSids

Элемент **GroupSids** представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory. 
  
```xml
<GroupSids>
   <GroupIdentifier/>
</GroupSids>
```

 **NonEmptyArrayOfGroupIdentifiersType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GroupIdentifier](groupidentifier.md) <br/> |Представляет одиночный идентификатор безопасности и атрибут, для которого учетная запись является участником группы объектов Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер. Сериализация маркера не поддерживается.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

