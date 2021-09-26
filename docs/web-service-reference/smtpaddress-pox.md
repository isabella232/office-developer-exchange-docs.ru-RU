---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит адрес SMTP, задаемый в хранилище сообщений общедоступных папок, настроенном для пользователя.
ms.openlocfilehash: d257b193a3254afceaa72d396a8c2724bb3165c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546989"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

Элемент **SmtpAddress содержит** адрес SMTP, задаемый в хранилище сообщений общедоступных папок, настроенном для пользователя. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
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
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Содержит сведения, которые клиенты могут использовать для отправки запроса автооткрытия для обнаружения общедоступных папок для пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет адрес SMTP, назначенный в хранилище общедоступных папок, настроенном для пользователя. Этот SMTP-адрес можно использовать в [элементе EMailAddress (POX)](emailaddress-pox.md) запроса автооткрытия для обнаружения параметров общедоступных папок. 
  
## <a name="remarks"></a>Заметки

Элемент **SmtpAddress** — это необходимый детский элемент элемента **PublicFolderInformation.** 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

