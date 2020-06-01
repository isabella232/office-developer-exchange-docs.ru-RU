---
title: UserId
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
description: Элемент UserId идентифицирует пользователя делегата или пользователя с разрешениями на доступ к папке.
ms.openlocfilehash: 68075e335383835ddce9575d85ba5fa945ed305c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455543"
---
# <a name="userid"></a>UserId

Элемент **UserID** идентифицирует пользователя делегата или пользователя с разрешениями на доступ к папке. 
  
```xml
<UserId>
   <SID/>
   <PrimarySmtpAddress/>
   <DisplayName/>
   <DistinguishedUser/>
   <ExternalUserIdentity/>
</UserId>
```

 **усеридтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SID](sid.md) <br/> |Представляет форму языка определения дескрипторов безопасности (SID).  <br/> |
|[PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной SMTP-адрес учетной записи, которая будет использоваться для делегирования доступа.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Определяет отображаемое имя папки, контакта, списка рассылки или пользователя делегата.  <br/> |
|[дистингуишедусер](distinguisheduser.md) <br/> |Определяет анонимные и учетные записи пользователей по умолчанию для делегирования доступа.  <br/> |
|[екстерналусеридентити](externaluseridentity.md) <br/> |Определяет внешнего пользователя делегата или внешнего пользователя с разрешениями на доступ к папке.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[делегатеусер](delegateuser.md) <br/> |Определяет одного делегата для добавления или обновления в почтовом ящике.  <br/> |
|[Разрешение](permission.md) <br/> |Определяет доступ пользователя к папке.  <br/> |
|[календарпермиссион](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря.  <br/> |
|[UserIds](userids.md) <br/> |Содержит массив делегированных пользователей, которые необходимо получить или удалить из почтового ящика участника.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
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

