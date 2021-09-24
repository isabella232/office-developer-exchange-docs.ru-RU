---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: Элемент RedirectTarget (SOAP) содержит цель URL-адреса перенаправления или адреса электронной почты.
ms.openlocfilehash: 0e09529f62dfde66f1ef05875bb0b0a0886db452
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513544"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

Элемент [RedirectTarget (SOAP)](redirecttarget-soap.md) содержит цель URL-адреса перенаправления или адреса электронной почты. 
  
```XML
<RedirectTarget/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос GetUserSettings для отдельного пользователя.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Содержит заданные параметры для указанного домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение содержит цель URL-адреса перенаправления или адреса электронной почты, которые следует использовать для последующего запроса GetUserSettings или GetDomainSettings.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

