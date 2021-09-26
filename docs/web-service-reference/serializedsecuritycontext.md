---
title: SerializedSecurityContext
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SerializedSecurityContext
api_type:
- schema
ms.assetid: a02c4fc1-ed1a-40d9-a18e-6cfdae21a690
description: Элемент SerializedSecurityContext используется в Протокол SOAP (SOAP) для сериализации маркеров в проверке подлинности от сервера к серверу. Сериализация маркеров не поддерживается.
ms.openlocfilehash: 55fe752813fc2d7e3ed5416401ff46b5e00516e3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546044"
---
# <a name="serializedsecuritycontext"></a>SerializedSecurityContext

Элемент **SerializedSecurityContext** используется в Протокол SOAP (SOAP) для сериализации маркеров при проверке подлинности от сервера к серверу. Сериализация маркеров не поддерживается. 
  
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
|[UserSid](usersid.md) <br/> |Представляет язык определения дескриптора безопасности (SDDL) идентификатора безопасности пользователя в заголовке SOAP контекста безопасности.  <br/> |
|[GroupSids](groupsids.md) <br/> |Представляет коллекцию идентификаторов объектов безопасности группы объектов службы каталогов Active Directory.  <br/> |
|[RestrictedGroupSids](restrictedgroupsids.md) <br/> |Представляет идентификатор безопасности группы и атрибуты для ограниченной группы.  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной простой протокол передачи почты (SMTP) учетной записи, используемой для авторизации от сервера к серверу.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который работает Microsoft Exchange Server 2007 г., где установлена роль сервера клиентского доступа (CAS).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Авторизация от сервера до сервера в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

