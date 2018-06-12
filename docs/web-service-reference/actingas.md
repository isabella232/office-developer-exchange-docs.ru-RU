---
title: ActingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: Элемент ActingAs определяет, как отправляющего вызывающего абонента.
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762510"
---
# <a name="actingas"></a>ActingAs

Элемент **ActingAs** определяет, как отправляющего вызывающего абонента. 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя. Этот элемент является необязательным.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Определяет маршрутизации, используемый для почтового ящика. Значение по умолчанию — SMTP. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetServiceConfiguration](getserviceconfiguration.md) <br/> |Определяет запрос **GetServiceConfiguration** .  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является необязательным. Если этот элемент не указан, прошедшего проверку пользователя считается отправителя. Элемент **ActingAs** должны быть включены для разрешения на запрос подсказки отправителя. Ошибка **ErrorInvalidArgument** можно получить в ответ, если элемент **ActingAs** отсутствует, не включает тип маршрутизации, не содержит адрес электронной почты, содержит недопустимый адрес электронной почты, не удается устранить для пользователей в Active Directory Доменных служб (AD DS) или разрешает нескольким пользователям в Доменных службах Active Directory. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

