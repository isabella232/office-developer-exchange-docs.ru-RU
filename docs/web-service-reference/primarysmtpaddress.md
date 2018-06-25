---
title: Параметр PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: Элемент PrimarySmtpAddress представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, используемые для проверки подлинности сервер сервер или передача прав доступа.
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834881"
---
# <a name="primarysmtpaddress"></a>Параметр PrimarySmtpAddress

Элемент **PrimarySmtpAddress** представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, используемые для проверки подлинности сервер сервер или передача прав доступа. 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Используется в заголовке SOAP для сериализации маркера проверки подлинности сервер сервер.  <br/> |
|[Идентификатор пользователя](userid.md) <br/> |Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее SMTP-адрес является обязательным.
  
## <a name="remarks"></a>Замечания

Веб-служб Exchange необходимо определить, что почтовые ящики по основной SMTP-адрес почтового ящика. Прокси-сервер или альтернативные адреса, не принимаются.
  
Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Сервер сервер авторизации в веб-служб Exchange](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[Работа с делегированный доступ](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

