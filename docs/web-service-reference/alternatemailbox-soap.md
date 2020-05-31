---
title: Алтернатемаилбокс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: Элемент Алтернатемаилбокс представляет альтернативный почтовый ящик.
ms.openlocfilehash: 8eb53e4846ad55916e2c5876606c00c0f2e371ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761425"
---
# <a name="alternatemailbox-soap"></a>Алтернатемаилбокс (SOAP)

Элемент **алтернатемаилбокс** представляет альтернативный почтовый ящик. 
  
```XML
<AlternateMailbox>
   <Type/>
   <DisplayName/>
   <LegacyDN/>
   <Server/>
   <SmtpAddress/>
</AlternateMailbox>
```

 **алтернатемаилбокс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Тип (SOAP)](type-soap.md) <br/> |Представляет альтернативный тип почтового ящика.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет альтернативное отображаемое имя почтового ящика.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Представляет альтернативное различающееся имя устаревшего почтового ящика.  <br/> |
|[Сервер (SOAP)](server-soap.md) <br/> |Представляет альтернативный сервер почтовых ящиков.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Представляет альтернативный SMTP-адрес почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Алтернатемаилбоксес (SOAP)](alternatemailboxes-soap.md) <br/> |Представляет коллекцию альтернативных почтовых ящиков.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Алтернатемаилбоксколлектионсеттинг (SOAP)](alternatemailboxcollectionsetting-soap.md)

