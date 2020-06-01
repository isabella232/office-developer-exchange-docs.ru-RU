---
title: Отклик (Жетдомаинсеттингс) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: Элемент Response представляет ответ на вызов Жетдомаинсеттингс для отдельного домена.
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455585"
---
# <a name="response-getdomainsettings-soap"></a>Отклик (Жетдомаинсеттингс) (SOAP)

Элемент **Response** представляет ответ на вызов **жетдомаинсеттингс** для отдельного домена. 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **жетдомаинсеттингсреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинреспонсес (SOAP)](domainresponses-soap.md) <br/> |Содержит ответ для каждого домена, запрошенного в запросе **жетдомаинсеттингс** .  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Содержит код ошибки, связанный с ответом (если это требуется).  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Содержит сообщение об ошибке, связанное с ответом (если это требуется).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетдомаинсеттингсреспонсемессаже (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Возврат к параметрам конфигурации домена, вызывающим абоненты.  <br/> |
   
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



[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

