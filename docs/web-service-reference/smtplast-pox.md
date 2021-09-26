---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: Элемент SMTPLast указывает, требует ли сервер Simple Mail Transfer Protocol (SMTP) загрузки электронной почты перед отправкой электронной почты с помощью сервера SMTP.
ms.openlocfilehash: ff1e47fa1e3ebd0267879cd596a3a559f2702943
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544684"
---
# <a name="smtplast-pox"></a>SMTPLast (POX)

Элемент **SMTPLast** указывает, требует ли сервер Simple Mail Transfer Protocol (SMTP) загрузки электронной почты перед отправкой электронной почты с помощью сервера SMTP. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [Protocol (POX)](protocol-pox.md)
  
- [SMTPLast (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server 2007 г., на который установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В текстовом значении указывается, требуется ли загрузка smTP-сервера электронной почты перед отправкой электронной почты с помощью сервера SMTP. Возможные значения **включаем и** **отключаем.** Значение по умолчанию **отключено.**
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

