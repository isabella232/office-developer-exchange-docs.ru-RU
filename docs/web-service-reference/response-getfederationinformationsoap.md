---
title: Отклик (Жетфедератионинформатион) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ca48a4b3-5006-4bb7-973e-d9137ce67e16
description: Элемент Response содержит сведения об отклике операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: 0b9a2c518b968faa6ef86b7c1f544eac40f8e5c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530588"
---
# <a name="response-getfederationinformation-soap"></a>Отклик (Жетфедератионинформатион) (SOAP)

Элемент **Response** содержит сведения об отклике [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<Response>
   <ErrorCode/>
   <ErrorMessage/>
   <ApplicationUri/>
   <Domains/>
</Response>
```

 **жетфедератионинформатионреспонсе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Представляет код ошибки, возвращенный службой автообнаружения.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.  <br/> |
|[ApplicationUri (SOAP)](applicationuri-soap.md) <br/> |Определяет расположение приложения.  <br/> |
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет коллекцию доменов, конфигурации, для которых выполняется [Операция жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), или домены, для которых в [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)используется федеративная организация.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетфедератионинформатионреспонсемессаже (SOAP)](getfederationinformationresponsemessage-soap.md) <br/> |Определяет ответ на запрос [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)

