---
title: Протоколконнектион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6eef2188-6194-48f1-ad7e-46104aecdf56
description: Элемент Протоколконнектион представляет подключение протокола для веб-клиента сервера.
ms.openlocfilehash: 8b5396821cd959e41d24fcf7a94c519f9c634a1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834915"
---
# <a name="protocolconnection-soap"></a>Протоколконнектион (SOAP)

Элемент **протоколконнектион** представляет подключение протокола для веб-клиента сервера. 
  
```XML
<ProtocolConnection>
   <Hostname/>
   <Port/>
   <EncryptionMethod/>
</ProtocolConnection>
```

 **протоколконнектион**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя узла (SOAP)](hostname-soap.md) <br/> |Представляет часть имени узла для полного имени компьютера.  <br/> |
|[Порт (SOAP)](port-soap.md) <br/> |Представляет номер порта, который будет использоваться для протокола.  <br/> |
|[EncryptionMethod (SOAP)](encryptionmethod-soap.md) <br/> |Представляет криптографический метод, используемый для протоколов POP, IMAP и SMTP.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протоколконнектионс (SOAP)](protocolconnections-soap.md) <br/> |Содержит ноль или более подключений протоколов.  <br/> |
   
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



[Протоколконнектионколлектионсеттинг (SOAP)](protocolconnectioncollectionsetting-soap.md)

