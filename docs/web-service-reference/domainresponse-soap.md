---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: Элемент DomainResponse содержит запрошенные параметры для конкретного домена.
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762207"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

Элемент **DomainResponse** содержит запрошенные параметры для конкретного домена. 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 **DomainResponse**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибке для параметров, которые не будут получены.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Определяет целевой в режиме одобрения администратором. Целевой объект может быть URL-адрес или адрес электронной почты.  <br/> |
|[Код ошибки (SOAP)](errorcode-soap.md) <br/> |Задает код ошибки, связанный с данным запросом.  <br/> |
|[Сообщение об ошибке (SOAP)](errormessage-soap.md) <br/> |Задает сообщение об ошибке, связанный с данным запросом.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Содержит массив элементов **DomainResponse** . Каждый элемент **DomainResponse** содержит запрошенные параметры для указанного пользователя.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Содержит ответы для каждого домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

