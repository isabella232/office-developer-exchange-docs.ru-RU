---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: Элемент DomainRequired указывает, требуется ли домен для проверки подлинности.
ms.openlocfilehash: 906c99ff7a8428404ee6045b749cdb0afed882b7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540064"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

Элемент **DomainRequired** указывает, требуется ли домен для проверки подлинности. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md) 
- [Account (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DomainRequired (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

Текстовое значение указывает, требуется ли домен для проверки подлинности. Возможные значения **включаем и** **отключаем.** Если значение в **значении,** последующий запрос должен содержать домен учетной записи пользователя.
  
## <a name="remarks"></a>Заметки

Если домен не указан в [элементе LoginName (POX)](loginname-pox.md) или элемент **LoginName** не указан, пользователь должен ввести домен, прежде чем проверка подлинности будет успешной. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

