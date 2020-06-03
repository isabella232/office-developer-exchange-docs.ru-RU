---
title: Домаинреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: Элемент Домаинреспонсе содержит запрошенные параметры для указанного домена.
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456964"
---
# <a name="domainresponse-soap"></a>Домаинреспонсе (SOAP)

Элемент **домаинреспонсе** содержит запрошенные параметры для указанного домена. 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 **домаинреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинсеттинжеррорс (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибках для параметров, которые не удалось вернуть.  <br/> |
|[Домаинсеттингс (SOAP)](domainsettings-soap.md) <br/> |Представляет параметры домена, которые были отправлены в запросе на обнаружение или возвращены ответом автообнаружения.  <br/> |
|[Редиректтаржет (SOAP)](redirecttarget-soap.md) <br/> |Указывает целевой объект перенаправления. Целевой может быть либо URL-адрес, либо адрес электронной почты.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Указывает код ошибки, связанный с конкретным запросом.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Указывает сообщение об ошибке, связанное с конкретным запросом.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Аррайофдомаинреспонсе (SOAP)](arrayofdomainresponse-soap.md) <br/> |Содержит массив элементов **домаинреспонсе** . Каждый элемент **домаинреспонсе** содержит запрошенные параметры для указанного пользователя.  <br/> |
|[Домаинреспонсес (SOAP)](domainresponses-soap.md) <br/> |Содержит ответы для каждого домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

