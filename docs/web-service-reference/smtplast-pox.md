---
title: Смтпласт (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: Элемент Смтпласт указывает, обязательно ли использовать SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера.
ms.openlocfilehash: 7019da28ffa196a9abc8798aa75aff2756198da3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468434"
---
# <a name="smtplast-pox"></a>Смтпласт (POX)

Элемент **смтпласт** указывает, обязательно ли использовать SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)
  
- [Ответ (POX)](response-pox.md)
  
- [Учетная запись (POX)](account-pox.md)
  
- [Протокол (POX)](protocol-pox.md)
  
- [Смтпласт (POX)](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает, требуется ли SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера. Возможные **значения:** **On и on** . Значение по умолчанию — " **отключено**".
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

