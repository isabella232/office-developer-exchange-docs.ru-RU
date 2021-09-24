---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: Элемент SmtpAddress представляет простой адрес протокола передачи почты (SMTP) учетной записи, используемой для олицетворения, или адреса получателя протокола передачи почты (SMTP) календаря или запроса на обмен контактами.
ms.openlocfilehash: c10e18ce77a1002a9c7a94718e8e9a2bd3877d8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539089"
---
# <a name="smtpaddress"></a>SmtpAddress

Элемент **SmtpAddress** представляет простой адрес протокола передачи почты (SMTP) учетной записи, используемой для олицетворения, или адреса получателя протокола передачи почты (SMTP) календаря или запроса на обмен контактами. 
  
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
|[ConnectingSID](connectingsid.md) <br/> |Представляет учетную запись для олицетворения при использовании мыла ExchangeImpersonation.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[InvalidRecipient](invalidrecipient.md) <br/> |Представляет недействительный получатель для общего доступа к календарю или сообщения общего доступа к контактам.  <br/> |
|[Recipients (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Представляет коллекцию получателей, которая получит доступ к общей папке.  <br/> |
|[GetSharingFolder](getsharingfolder.md) <br/> |Определяет запрос для получения локального идентификатора папки указанной общей папки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение, представляю которое представляет smTP-адрес.
  
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге IIS, Exchange веб-службы компьютера, на котором Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

