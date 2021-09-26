---
title: EcpUrl-extinstall (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: f81807e6-93de-4e47-afee-1e1ae6a85054
description: Элемент EcpUrl-extinstall указывает частичный URL-адрес, который можно сочетать со значением элемента EcpUrl (POX) для создания URL-адреса, который можно использовать для просмотра или изменения почтовых приложений, установленных в почтовом ящике пользователя.
ms.openlocfilehash: bf91b12cbcff3b08b3b13569eac9c957dea12757
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541422"
---
# <a name="ecpurl-extinstall-pox"></a>EcpUrl-extinstall (POX)

Элемент **EcpUrl-extinstall** указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для просмотра или изменения почтовых приложений, установленных в почтовом ящике пользователя. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md)
  
```XML
<EcpUrl-extinstall/>
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

Текстовое значение представляет частичный URL-адрес, который можно сочетать со значением элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для просмотра или изменения почтовых приложений, установленных в почтовом ящике пользователя. 
  
## <a name="remarks"></a>Заметки

Элемент **EcpUrl-extinstall** является необязательным детским элементом элемента **Protocol.** 
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

