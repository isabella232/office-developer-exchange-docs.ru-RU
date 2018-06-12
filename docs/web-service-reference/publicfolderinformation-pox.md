---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: Элемент PublicFolderInformation содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834927"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

Элемент **PublicFolderInformation** содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
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
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Содержит SMTP-адрес, назначенный хранилище сообщений общих папок, настраиваемый для пользователя. SMTP-адреса можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса службы автообнаружения для обнаружения параметров общей папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Учетная запись (POX)](account-pox.md) <br/> |Задает параметры учетной записи пользователя.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **PublicFolderInformation** является необязательным дочерним элементом элемента **учетной записи** . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

