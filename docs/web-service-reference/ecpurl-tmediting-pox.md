---
title: EcpUrl-tmEditing (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: Элемент EcpUrl tmEditing указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента EcpUrl (POX) для создания URL-адрес, который может использоваться для изменения существующего почтового ящика сайта.
ms.openlocfilehash: 29b27ffe9ef3c18a3b6471ca4a42956a43a5aaa6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762246"
---
# <a name="ecpurl-tmediting-pox"></a>EcpUrl-tmEditing (POX)

Элемент **EcpUrl tmEditing** указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который может использоваться для изменения существующего почтового ящика сайта. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
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

Текстовое значение представляет сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который может использоваться для изменения существующего почтового ящика сайта. Значение элемента **EcpUrl tmEditing** содержит параметры, содержащиеся в "<" и ">" символы, которые заменяются клиентом, как показано в следующей таблице. 
  
|**Параметр**|**Заменить**|
|:-----|:-----|
| 
  _Id_ <br/> |Адрес электронной почты SMTP или X500 различающееся имя почтового ящика сайта.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **EcpUrl tmEditing** является необязательным дочерним элементом элемента **протокола** . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

