---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: Элемент EcpUrl tmHiding указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента EcpUrl (POX) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта.
ms.openlocfilehash: 461e9780dbd657ba0ba8b9ce9ea4fe902cba9698
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762248"
---
# <a name="ecpurl-tmhiding-pox"></a>EcpUrl-tmHiding (POX)

Элемент **EcpUrl tmHiding** указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта. Значение элемента **EcpUrl tmHiding** содержит параметры, содержащиеся в "<" и ">" символы, которые заменяются клиентом, как показано в следующей таблице. 
  
|**Параметр**|**Заменить**|
|:-----|:-----|
| 
  _Id_ <br/> |Адрес электронной почты SMTP или X500 различающееся имя почтового ящика сайта.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **EcpUrl tmHiding** является необязательным дочерним элементом элемента **протокола** . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

