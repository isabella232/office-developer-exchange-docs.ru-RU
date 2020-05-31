---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835507"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

Элемент **SmtpAddress** содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
  
- [Ответ (POX)](response-pox.md)
  
- [Учетная запись (POX)](account-pox.md)
  
- [Публикфолдеринформатион (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Публикфолдеринформатион (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет SMTP-адрес, назначенный хранилищу общедоступных папок, настроенному для пользователя. Этот SMTP-адрес можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса на автообнаружение для обнаружения параметров общедоступных папок. 
  
## <a name="remarks"></a>Примечания

Элемент **SmtpAddress** является обязательным дочерним элементом элемента **публикфолдеринформатион** . 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

