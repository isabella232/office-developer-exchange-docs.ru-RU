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
ms.openlocfilehash: b9df3febe36db53d7c5bf0610ba857f13aa96abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528862"
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

Отсутствуют.
  
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

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Протоколконнектионколлектионсеттинг (SOAP)](protocolconnectioncollectionsetting-soap.md)

