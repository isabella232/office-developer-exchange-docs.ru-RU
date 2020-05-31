---
title: Публикфолдеринформатион (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: Элемент Публикфолдеринформатион содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834927"
---
# <a name="publicfolderinformation-pox"></a>Публикфолдеринформатион (POX)

Элемент **публикфолдеринформатион** содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Публикфолдеринформатион (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя. Этот SMTP-адрес можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса на автообнаружение для обнаружения параметров общедоступных папок.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Учетная запись (POX)](account-pox.md) <br/> |Задает параметры учетной записи пользователя.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **публикфолдеринформатион** является необязательным дочерним элементом элемента **Account** . 
  
## <a name="see-also"></a>См. также



[XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

