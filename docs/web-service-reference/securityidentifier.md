---
title: секуритидентифиер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SecurityIdentifier
api_type:
- schema
ms.assetid: f7656729-f2c9-41cc-b1ec-60f480fc4dab
description: Элемент Секуритидентифиер представляет форму языка определения дескрипторов безопасности (SID).
ms.openlocfilehash: c18d7d4505c618792497c32c7499eab9ac82989e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835314"
---
# <a name="securityidentifier"></a>секуритидентифиер

Элемент **секуритидентифиер** представляет форму языка определения дескрипторов безопасности ( [SID](sid.md)).
  
```xml
<SecurityIdentifier/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[граупидентифиер](groupidentifier.md) <br/> |Представляет один идентификатор безопасности и атрибут для группы объектов Active Directory, членом которой является учетная запись.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/SerializedSecurityContext/GroupSids/GroupIdentifier[i]` <br/> |
|[рестриктедграупидентифиер](restrictedgroupidentifier.md) <br/> |Представляет идентификатор и атрибуты безопасности группы для группы с ограниченным доступом в маркере пользователя.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент используется в заголовке протокола SOAP.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

