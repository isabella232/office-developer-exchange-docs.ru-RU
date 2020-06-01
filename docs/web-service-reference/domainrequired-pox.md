---
title: Домаинрекуиред (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: Элемент Домаинрекуиред указывает, требуется ли домен для проверки подлинности.
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461326"
---
# <a name="domainrequired-pox"></a>Домаинрекуиред (POX)

Элемент **домаинрекуиред** указывает, требуется ли домен для проверки подлинности. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md) 
- [Учетная запись (POX)](account-pox.md)  
- [Протокол (POX)](protocol-pox.md)  
- [Домаинрекуиред (POX)](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
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

Текстовое значение указывает, требуется ли домен для проверки подлинности. Возможные **значения:** **On и on** . Если значение равно **On**, то следующий запрос должен содержать домен учетной записи пользователя.
  
## <a name="remarks"></a>Примечания

Если домен не указан в элементе [LoginName (POX)](loginname-pox.md) или элемент **LoginName** не был указан, пользователь должен ввести домен, прежде чем проверка подлинности будет выполнена. 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

