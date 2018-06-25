---
title: PrincipalName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrincipalName
api_type:
- schema
ms.assetid: 88c142d4-0bc7-43ea-a997-d7200664d900
description: Элемент PrincipalName представляет имя участника-пользователя (UPN) учетной записи, которая будет использоваться для олицетворения Exchange.
ms.openlocfilehash: d8557ce0435a11a5602372517db1f576028a9c97
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834882"
---
# <a name="principalname"></a>PrincipalName

Элемент **PrincipalName** представляет имя участника-пользователя (UPN) учетной записи, которая будет использоваться для олицетворения Exchange. 
  
```xml
<PrincipalName/>
```

 **PrincipalNameType**
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
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет имя участника-пользователя. Это значение существует в объекте пользователя в службе каталогов Active Directory. Содержит имя входа пользователя и имя домена, которое определяет домен, в котором расположена учетная запись пользователя, в следующем формате: `someone@example.com`.
  
## <a name="remarks"></a>Замечания

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

