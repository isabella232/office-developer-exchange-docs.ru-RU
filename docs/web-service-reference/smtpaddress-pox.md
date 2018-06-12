---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит SMTP-адрес, назначенный хранилище сообщений общих папок, настраиваемый для пользователя.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835507"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

Элемент **SmtpAddress** содержит SMTP-адрес, назначенный хранилище сообщений общих папок, настраиваемый для пользователя. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)
  
- [Ответ (POX)](response-pox.md)
  
- [Учетная запись (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет SMTP-адрес, назначенный хранилище общих папок, настроенных для пользователя. SMTP-адреса можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса службы автообнаружения для обнаружения параметров общей папки. 
  
## <a name="remarks"></a>Замечания

Элемент **SmtpAddress** является обязательным дочерним элементом элемента **PublicFolderInformation** . 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

