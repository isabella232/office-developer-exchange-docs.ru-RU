---
title: ИД пользователя
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserId
api_type:
- schema
ms.assetid: 244af9e0-bf3c-46b4-8bfa-9719a1ed3107
description: Элемент UserId определяет представитель или пользователь, имеющий права доступа к папкам.
ms.openlocfilehash: 8e9867f5a8cdd62dd2dae55fbf527595ac14f46d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840421"
---
# <a name="userid"></a>ИД пользователя

Элемент **UserId** определяет представитель или пользователь, имеющий права доступа к папкам. 
  
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
|[ИД БЕЗОПАСНОСТИ](sid.md) <br/> |Представляет идентификатор безопасности (SID) формы языке SDDL определения дескриптора безопасности.  <br/> |
|[Параметр PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для доступа делегата.  <br/> |
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Задает отображаемое имя папки, контактов, список рассылки или делегата.  <br/> |
|[DistinguishedUser](distinguisheduser.md) <br/> |Определяет учетные записи пользователей анонимные пользователи и по умолчанию для доступа делегата.  <br/> |
|[ExternalUserIdentity](externaluseridentity.md) <br/> |Идентифицирует пользователя с внешним делегат или внешний пользователь, имеющий права доступа к папкам.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DelegateUser](delegateuser.md) <br/> |Определяет один делегат для добавления или обновления в почтовом ящике.  <br/> |
|[Разрешение](permission.md) <br/> |Определяет доступ пользователя к папке.  <br/> |
|[CalendarPermission](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря.  <br/> |
|[UserIds](userids.md) <br/> |Содержит массив делегат пользователям получить или удалить из почтового ящика участника.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция AddDelegate](adddelegate-operation.md)
  
[Операция UpdateDelegate](updatedelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

