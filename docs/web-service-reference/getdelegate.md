---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: Элемент GetDelegate определяет запрос на получение сведений о делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e31d6bd4f4387094beb467fcc4dff31ca7ec5d62
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762745"
---
# <a name="getdelegate"></a>GetDelegate

Элемент **GetDelegate** определяет запрос на получение сведений о делегатов к почтовому ящику. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 **GetDelegateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IncludePermissions** <br/> |Показывает, содержит ли ответ параметры разрешений для каждого пользователя делегатом.  <br/> |
   
#### <a name="includepermissions-attribute-values"></a>Значения атрибутов IncludePermissions

|**Значение**|**Описание**|
|:-----|:-----|
|**Значение true** <br/> |Делегирование пользователя, в дополнение к информации пользователя делегата, который возвращается в элемент [UserId](userid.md) возвращаются разрешения.  <br/> |
|**Значение false** <br/> |Возвращается информация [идентификатор пользователя](userid.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет основного сервера почтовых ящиков.  <br/> |
|[UserIds](userids.md) <br/> |Содержит массив делегат пользователям получать из почтового ящика участника. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetDelegate](getdelegate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

