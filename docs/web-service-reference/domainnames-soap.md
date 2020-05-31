---
title: Имя_домена (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: Элемент DomainNames представляет коллекцию доменных имен. Элемент DomainNames предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 45d256f3d5a57028a04572ad67d4be0786ca39e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762205"
---
# <a name="domainnames-soap"></a>Имя_домена (SOAP)

Элемент **domainnames** представляет коллекцию доменных имен. Элемент **domainnames** предназначен только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 **Имя_домена**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет коллекцию доменов, которые возвращаются из [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)или [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Организатионрелатионшипсеттингс (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений Организации для одной организации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Этот элемент представляет домены SMTP внешних организаций.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

