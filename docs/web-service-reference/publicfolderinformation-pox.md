---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: Элемент PublicFolderInformation содержит сведения, которые клиенты могут использовать для отправки запроса автообнаружения для обнаружения общедоступных папок для пользователя.
ms.openlocfilehash: d77ea350f05c5d6137d3b67cfd49119bf9590e53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540624"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

Элемент **PublicFolderInformation содержит** сведения, которые клиенты могут использовать для отправки запроса автообнаружения для обнаружения общедоступных папок для пользователя. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Содержит адрес SMTP, назначенный в хранилище сообщений общедоступных папок, настроенный для пользователя. Этот SMTP-адрес можно использовать в [элементе EMailAddress (POX)](emailaddress-pox.md) запроса автооткрытия для обнаружения параметров общедоступных папок.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Указывает параметры учетной записи для пользователя.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **PublicFolderInformation** — необязательный детский элемент элемента **Учетная** запись. 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

