---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: Элемент DomainRequired указывает, является ли домена для проверки подлинности требуется.
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762204"
---
# <a name="domainrequired-pox"></a>DomainRequired (POX)

Элемент **DomainRequired** указывает, является ли домена для проверки подлинности требуется. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md) 
- [Учетная запись (POX)](account-pox.md)  
- [Протокол (POX)](protocol-pox.md)  
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение указывает, необходима ли домена для проверки подлинности. Возможные значения: **и **отключает**** . Если значение **на**следующий запрос должен содержать домен учетной записи пользователя.
  
## <a name="remarks"></a>Замечания

Если домен не указан в элементе [LoginName (POX)](loginname-pox.md) или элемент **LoginName** не указан, пользователя необходимо ввести домен будет успешной проверки подлинности. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

