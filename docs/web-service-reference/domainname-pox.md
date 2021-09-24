---
title: DomainName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: Элемент DomainName указывает домен пользователя.
ms.openlocfilehash: 9242c867d684bf9803f8c6ed1082d578cca05505
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526435"
---
# <a name="domainname-pox"></a>DomainName (POX)

Элемент **DomainName** указывает домен пользователя. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)  
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md) 
- [Protocol (POX)](protocol-pox.md) 
- [DomainName (POX)](domainname-pox.md)
  
```xml
<DomainName/>
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

Текстовое значение указывает домен пользователя.
  
## <a name="remarks"></a>Заметки

Если значение не задано, проверка подлинности по умолчанию используется для использования адреса электронной почты в качестве основного имени пользователя (UPN). Например: \<Username\> @ \<Domain\> .
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

