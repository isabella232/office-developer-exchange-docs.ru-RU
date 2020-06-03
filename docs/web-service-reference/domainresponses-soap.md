---
title: Домаинреспонсес (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: Элемент Домаинреспонсес содержит массив ответов для каждого параметра запрашиваемого домена.
ms.openlocfilehash: 2c76b9691fe88657a65130ef6829e5af64380d95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526321"
---
# <a name="domainresponses-soap"></a>Домаинреспонсес (SOAP)

Элемент **домаинреспонсес** содержит массив ответов для каждого параметра запрашиваемого домена. 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 **аррайофдомаинреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинреспонсе (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для указанного домена.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетдомаинсеттингсреспонсе (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Представляет ответ на запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) для домена и возвращает параметры домена.  <br/> |
|[Отклик (Жетдомаинсеттингс) (SOAP)](response-getdomainsettingssoap.md) <br/> |Представляет ответ на вызов [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) для отдельного домена.  <br/> |
   
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

