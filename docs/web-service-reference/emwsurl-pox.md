---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: Элемент EmwsUrl указывает URL-адрес наилучшего экземпляра конечной точки для Exchange веб-служб (EWS) для пользователя с поддержкой почты.
ms.openlocfilehash: d46438f600e226bce95c5e479aca91bfa942535e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538177"
---
# <a name="emwsurl-pox"></a>EmwsUrl (POX)

Элемент **EmwsUrl** указывает URL-адрес наилучшего экземпляра конечной точки для Exchange веб-служб (EWS) для пользователя с поддержкой почты. 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
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
|[Protocol (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к компьютеру, на Microsoft Exchange Server установлена роль сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет URL-адрес конечной точки EWS для пользователя. Он эквивалентен элементу [EwsUrl (POX).](ewsurl-pox.md) 
  
## <a name="remarks"></a>Заметки

Элемент **EmwsUrl является** необязательным детским элементом **элемента Protocol.** 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

