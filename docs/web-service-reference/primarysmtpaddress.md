---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: Элемент PrimarySmtpAddress представляет основной простой адрес протокола передачи почты (SMTP) учетной записи, используемой для авторизации или делегирования доступа к серверу.
ms.openlocfilehash: 7963fbc92de88b38da93e577ebd2c39dbedac009
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523876"
---
# <a name="primarysmtpaddress"></a>PrimarySmtpAddress

Элемент **PrimarySmtpAddress** представляет основной простой адрес протокола передачи почты (SMTP) учетной записи, используемой для авторизации или делегирования доступа к серверу. 
  
```xml
<PrimarySmtpAddress/>
```

 **PrimarySmtpAddressType**
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
|[SerializedSecurityContext](serializedsecuritycontext.md) <br/> |Используется в загонах SOAP для сериализации маркеров в проверке подлинности от сервера к серверу.  <br/> |
|[UserId](userid.md) <br/> |Определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение, представляю которое представляет smTP-адрес.
  
## <a name="remarks"></a>Заметки

Exchange Веб-службы требуют, чтобы почтовые ящики были идентифицированы по основному SMTP-адресу почтового ящика. Прокси или альтернативные адреса не принимаются.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Авторизация от сервера до сервера в EWS](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[Работа с доступом к делегатам](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

