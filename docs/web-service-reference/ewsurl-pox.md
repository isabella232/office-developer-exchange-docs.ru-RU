---
title: EwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73cebc8c-770a-4f1b-b93e-51e7e2f3e342
description: Элемент EwsUrl указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: c968b13a069cdc15803c1eb491244b4dc1aa422f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762410"
---
# <a name="ewsurl-pox"></a>EwsUrl (POX)

Элемент **EwsUrl** указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты. 
  
[Автообнаружение (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[EwsUrl (POX)](ewsurl-pox.md)
  
```XML
<EwsUrl/>
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

Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.
  
## <a name="remarks"></a>Замечания

Элемент **EwsUrl** является необязательным дочерним элементом элемента **протокола** . 
  
## <a name="see-also"></a>См. также



[Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

