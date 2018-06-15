---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: Элемент AlternateMailbox представляет альтернативного почтового ящика.
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/15/2018
ms.locfileid: "19761425"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

Элемент **AlternateMailbox** представляет альтернативного почтового ящика. 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 **AlternateMailbox**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тип (SOAP)](type-soap.md) <br/> |Представляет тип альтернативного почтового ящика.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет отображаемое имя альтернативного почтового ящика.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Представляет устаревшее различающееся имя альтернативного почтового ящика.  <br/> |
|[Сервер (SOAP)](server-soap.md) <br/> |Представляет сервер альтернативного почтового ящика.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Представляет альтернативного SMTP-адрес почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Представляет коллекцию альтернативного почтовых ящиков.  <br/> |
   
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

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

