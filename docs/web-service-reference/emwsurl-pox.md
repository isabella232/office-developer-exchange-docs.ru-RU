---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: Элемент EmwsUrl указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762328"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

Элемент **EmwsUrl** указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты. 
  
- [Автообнаружение (POX)](autodiscover-pox.md) 
- [Ответ (POX)](response-pox.md) 
- [Учетная запись (POX)](account-pox.md) 
- [Протокол (POX)](protocol-pox.md) 
- [EmwsUrl (POX)](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
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

Текстовое значение представляет URL-адрес конечной точки EWS для пользователя. Это эквивалентно элемент [EwsUrl (POX)](ewsurl-pox.md) . 
  
## <a name="remarks"></a>Замечания

Элемент **EmwsUrl** является необязательным дочерним элементом элемента **протокола** . 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

