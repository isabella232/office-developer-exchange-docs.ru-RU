---
title: Редиректтаржет (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: Элемент Редиректтаржет (SOAP) содержит целевой объект URL-адреса перенаправления или адреса электронной почты.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835019"
---
# <a name="redirecttarget-soap"></a>Редиректтаржет (SOAP)

Элемент [редиректтаржет (SOAP)](redirecttarget-soap.md) содержит целевой объект URL-адреса перенаправления или адреса электронной почты. 
  
```XML
<RedirectTarget/>
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
|[Усерреспонсе (SOAP)](userresponse-soap.md) <br/> |Представляет ответ на запрос GetUserSettings для отдельного пользователя.  <br/> |
|[Домаинреспонсе (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для указанного домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение содержит целевой объект URL-адреса перенаправления или адрес электронной почты, который должен использоваться для последующего запроса GetUserSettings или Жетдомаинсеттингс.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

