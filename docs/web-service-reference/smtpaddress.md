---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: Элемент SmtpAddress представляет адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для олицетворения или адрес получателя Simple Mail Transfer Protocol (SMTP), календаря или контакта, запрос на общий доступ.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835511"
---
# <a name="smtpaddress"></a>SmtpAddress

Элемент **SmtpAddress** представляет адрес Simple Mail Transfer Protocol (SMTP) учетной записи, которое будет использоваться для олицетворения или адрес получателя Simple Mail Transfer Protocol (SMTP), календаря или контакта, запрос на общий доступ. 
  
```xml
<SmtpAddress/>
```

**SmtpAddressType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ConnectingSID](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Представляет недопустимого получателя общий доступ к календарю или контакта, общий доступ к сообщения.  <br/> |
|[Получатели (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Представляет коллекцию получателей, которым будет предоставлен доступ к общей папке.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Определяет запрос на получение идентификатора локальной папки указанной общей папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее SMTP-адрес является обязательным.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

