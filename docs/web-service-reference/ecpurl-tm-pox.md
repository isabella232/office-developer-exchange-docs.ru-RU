---
title: EcpUrl-tm (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 3f35d5ac-55be-4d3a-ad03-7d6e9349d923
description: Элемент EcpUrl-tm указывает частичный URL-адрес, который можно сочетать со значением элемента EcpUrl (POX) для создания URL-адреса, который можно использовать для доступа к списку всех почтовых ящиков сайтов, членом которых в настоящее время является пользователь с поддержкой почты.
ms.openlocfilehash: 5d24a198a3466bb84e14f925e4b6fa15fa229b24
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526307"
---
# <a name="ecpurl-tm-pox"></a>EcpUrl-tm (POX)

Элемент **EcpUrl-tm** указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к списку всех почтовых ящиков сайтов, членом которых в настоящее время является пользователь с поддержкой почты. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-tm (POX)](ecpurl-tm-pox.md)
  
```XML
<EcpUrl-tm/>
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к списку почтовых ящиков сайта для пользователя. 
  
## <a name="remarks"></a>Заметки

Элемент **EcpUrl-tm** является необязательным детским элементом элемента **Protocol.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

