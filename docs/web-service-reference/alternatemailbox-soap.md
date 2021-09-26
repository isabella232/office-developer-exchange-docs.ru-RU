---
title: AlternateMailbox (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d913a70d-5a85-4b6e-becc-2fb9334b6088
description: Элемент AlternateMailbox представляет альтернативный почтовый ящик.
ms.openlocfilehash: 3646efef9b63b2af8dbba41a07a86462e18ac1c1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543725"
---
# <a name="alternatemailbox-soap"></a>AlternateMailbox (SOAP)

Элемент **AlternateMailbox** представляет альтернативный почтовый ящик. 
  
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
|[Type (SOAP)](type-soap.md) <br/> |Представляет альтернативный тип почтового ящика.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет альтернативное имя отображения почтового ящика.  <br/> |
|[LegacyDN (SOAP)](legacydn-soap.md) <br/> |Представляет альтернативное имя почтового ящика.  <br/> |
|[Server (SOAP)](server-soap.md) <br/> |Представляет альтернативный сервер почтовых ящиков.  <br/> |
|[SmtpAddress (SOAP)](smtpaddress-soap.md) <br/> |Представляет альтернативный адрес SMTP почтового ящика.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AlternateMailboxes (SOAP)](alternatemailboxes-soap.md) <br/> |Представляет коллекцию альтернативных почтовых ящиков.  <br/> |
   
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

- [AlternateMailboxCollectionSetting (SOAP)](alternatemailboxcollectionsetting-soap.md)

