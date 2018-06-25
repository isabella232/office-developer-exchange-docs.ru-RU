---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: Элемент WebClientUrl представляет URL-адрес веб-клиент Exchange.
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840502"
---
# <a name="webclienturl-soap"></a>WebClientUrl (SOAP)

Элемент **WebClientUrl** представляет URL-адрес веб-клиент Exchange. 
  
[UserSetting (SOAP)](usersetting-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)
  
[WebClientUrl (SOAP)](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 **WebClientUrl**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AuthenticationMethods (SOAP)](authenticationmethods-soap.md) <br/> |Представляет метод проверки подлинности для использования при доступе к указанному URL-АДРЕСУ.  <br/> |
|[URL-адрес (SOAP)](url-soap.md) <br/> |Представляет веб-адрес, URL-адреса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[WebClientUrls (SOAP)](webclienturls-soap.md) <br/> |Представляет параметр пользователя, который содержит коллекцию элементов **WebClientUrl** .  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[URL-адрес (SOAP)](url-soap.md)
  
[WebClientUrls (SOAP)](webclienturls-soap.md)

