---
title: ConnectingSID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectingSID
api_type:
- schema
ms.assetid: 56d6aa52-8fa6-4773-9046-44a6f4f5d97c
description: Элемент ConnectingSID представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.
ms.openlocfilehash: 6e0bb90e197ce22bcd982a6d51954a88f3a2cf03
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761720"
---
# <a name="connectingsid"></a>ConnectingSID

Элемент **ConnectingSID** представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP. 
  
[ExchangeImpersonation](exchangeimpersonation.md)
  
[ConnectingSID](connectingsid.md)
  
```xml
<ConnectingSID>
   <PrincipalName/>
</ConnectingSID>
```

 **ConnectingSIDType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PrincipalName](principalname.md) <br/> |Представляет имя участника-пользователя (UPN) учетную запись, используемую для олицетворения. Это должно быть имя участника-пользователя для домена, где существует учетная запись пользователя.  <br/> |
|[ИД БЕЗОПАСНОСТИ](sid.md) <br/> |Представляет идентификатор безопасности (SID) формы языке SDDL определения дескриптор безопасности для учетной записи для использования при олицетворении.  <br/> |
|[Параметр PrimarySmtpAddress](primarysmtpaddress.md) <br/> |Представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетную запись, используемую для олицетворения Exchange. Если предоставлен основной SMTP-адрес, это потребует дополнительного поиска службы каталогов Active Directory для получения ИД безопасности пользователя. Мы рекомендуем использовать ИД безопасности или имя участника-пользователя, если они доступны.  <br/> |
|[SmtpAddress](smtpaddress.md) <br/> |Представляет адрес Simple Mail Transfer Protocol (SMTP) учетную запись, используемую для олицетворения Exchange. Если предоставлен SMTP-адрес, это потребует дополнительного поиска Active Directory для получения ИД безопасности пользователя. Мы рекомендуем использовать ИД безопасности или имя участника-пользователя, если они доступны.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Используется в заголовке SOAP запроса. Если этот элемент, вызывающего абонента пытается олицетворить учетную запись, которая содержится в элементе **ExchangeImpersonation** .  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/ExchangeImpersonation` <br/> |
   
## <a name="remarks"></a>Замечания

Вызывающий учетная запись должна иметь **ms-exch-impersonation** непосредственно на сервер клиентского доступа и **ms-exch-MayImpersonate** непосредственно в либо базы данных почтовых ящиков, почтовых ящиков для олицетворения или Active Directory пользователя или контакта объект. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Сервер сервер авторизации в веб-служб Exchange](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

