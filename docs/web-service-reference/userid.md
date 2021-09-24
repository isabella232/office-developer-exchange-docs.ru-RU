---
title: UserId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: Элемент UserId определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам.
ms.openlocfilehash: f03914745f8f7f47c64685b3e7c52eefece5ff6d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510759"
---
# <a name="userid"></a>UserId

Элемент **UserId** определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам. 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **UserIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SID](sid.md) <br/> |Представляет язык определения дескриптора безопасности (SDDL) формы идентификатора безопасности (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной простой протокол передачи почты (SMTP) учетной записи, используемой для делегирования доступа.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Определяет имя отображения папки, контакта, списка рассылки или пользователя делегирования.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Определяет учетные записи пользователей Anonymous и Default для доступа к делегатам.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Идентифицирует внешнего пользователя делегирования или внешнего пользователя, у которого есть разрешения на доступ к папке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Определяет одного делегата для добавления или обновления в почтовом ящике.  <br/> |
|[Разрешение](permission.md) <br/> |Определяет доступ пользователя к папке.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря.  <br/> |
|[UserIds](userids.md) <br/> |Содержит массив пользователей делегирования для получения или удаления из почтового ящика директора.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

