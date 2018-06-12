---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: Элемент SerializedSecurityContext используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер. Сериализация маркера не поддерживается.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835363"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

Элемент **SerializedSecurityContext** используется в заголовке Simple Object Access Protocol (SOAP) для сериализации маркера проверки подлинности сервер сервер. Сериализация маркера не поддерживается. 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **SerializedSecurityContextType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserSid](usersid.md) <br/> |Представляет форме безопасности определения дескриптора языке SDDL идентификатор безопасности пользователя в заголовке SOAP контекста сериализованных безопасности.  <br/> |
|[GroupSids](groupsids.md) <br/> |Представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Представляет идентификатор группы безопасности и атрибуты, используемые для группа с ограниченным доступом.  <br/> |
|[Параметр PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для проверки подлинности сервер сервер.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера (CAS) клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Сервер сервер авторизации в веб-служб Exchange](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

