---
title: Жетфедератионинформатионреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2033c14f-dcc8-43c2-9fd9-a51946ec7055
description: Элемент Жетфедератионинформатионреспонсе содержит ответ операции Жетфедератионинформатион (SOAP).
ms.openlocfilehash: c9e65a2b1759946b8493b3c730f08df6fe353fd8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460045"
---
# <a name="getfederationinformationresponse-soap"></a>Жетфедератионинформатионреспонсе (SOAP)

Элемент **жетфедератионинформатионреспонсе** содержит ответ [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) . 
  
```XML
<GetFederationInformationResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <TokenIssuers/>
   <ApplicationUri/>
   <Domains/>
</GetFederationInformationResponse>
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
|[Токениссуерс (SOAP)](tokenissuers-soap.md) <br/> |Представляет коллекцию маркеров безопасности, которая содержит идентификаторы и конечные точки службы маркеров безопасности.  <br/> |
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет домены, для которых в операции [жетфедератионинформатион (SOAP) операции (SOAP)](getfederationinformation-operation-soap.md) **жетфедератионинформатион** операции, которые возвращаются в ходе операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) **жетдомаинсеттингс** или домены, в которых участвует Организация.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
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



[Операция Жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)

