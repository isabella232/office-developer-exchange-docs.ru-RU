---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: Элемент DomainResponse содержит запрашиваемую настройку указанного домена.
ms.openlocfilehash: fb7288b55452d8499596ce09c3ada9cec4b88d5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517205"
---
# <a name="domainresponse-soap"></a>DomainResponse (SOAP)

Элемент **DomainResponse содержит** запрашиваемую настройку указанного домена. 
  
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
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибках для параметров, которые не удалось вернуть.  <br/> |
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Представляет параметры домена, которые были отправлены в запросе автооткрытия или возвращены ответом автооткрытия.  <br/> |
|[RedirectTarget (SOAP)](redirecttarget-soap.md) <br/> |Определяет цель перенаправления. Целью может быть URL-адрес или адрес электронной почты.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Указывает код ошибки, связанный с определенным запросом.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Указывает сообщение об ошибке, связанное с определенным запросом.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ArrayOfDomainResponse (SOAP)](arrayofdomainresponse-soap.md) <br/> |Содержит массив **элементов DomainResponse.** Каждый **элемент DomainResponse** содержит заданные параметры для указанного пользователя.  <br/> |
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Содержит ответы для каждого домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

