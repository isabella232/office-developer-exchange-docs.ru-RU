---
title: сериализедсекуритиконтекст
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
description: Элемент Сериализедсекуритиконтекст используется в заголовке протокола SOAP для сериализации маркеров при проверке подлинности "сервер-сервер". Сериализация маркеров не поддерживается.
ms.openlocfilehash: c5590551dc0780d918b05902e4f48fb9d1390b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835363"
---
# <a name="serializedsecuritycontext"></a>сериализедсекуритиконтекст

Элемент **сериализедсекуритиконтекст** используется в заголовке протокола SOAP для сериализации маркеров при проверке подлинности "сервер-сервер". Сериализация маркеров не поддерживается. 
  
```xml
<SerializedSecurityContext>
   <UserSid/>
   <GroupSids/>
   <RestrictedGroupSids/>
   <PrimarySmtpAddress/>
</SerializedSecurityContext>
```

 **сериализедсекуритиконтексттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[О.](usersid.md) <br/> |Представляет форму языка определения дескрипторов безопасности (SDDL) для идентификатора безопасности пользователя в сериализованном SOAP-заголовке контекста безопасности.  <br/> |
|[граупсидс](groupsids.md) <br/> |Представляет коллекцию идентификаторов безопасности объектов группы службы каталогов Active Directory.  <br/> |
|[рестриктедграупсидс](restrictedgroupsids.md) <br/> |Представляет идентификатор и атрибуты безопасности группы для группы с ограниченным доступом.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер".  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа (CAS).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Авторизация между серверами в EWS](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

