---
title: Имя домена (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: Элемент DomainName указывает пользователя домена.
ms.openlocfilehash: c38d2e470bd174ab6dd7e5e1dd3eee23daea5e69
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762208"
---
# <a name="domainname-pox"></a>Имя домена (POX)

Элемент **DomainName** указывает пользователя домена. 
  
- [Автообнаружение (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md)  
- [Учетная запись (POX)](account-pox.md) 
- [Протокол (POX)](protocol-pox.md) 
- [Имя домена (POX)](domainname-pox.md)
  
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение определяет пользователя домена.
  
## <a name="remarks"></a>Замечания

Если значение не указано, проверки подлинности по умолчанию является использование адрес электронной почты в формате имя участника (UPN) пользователя. Например: \<Username\>@\<домена\>.
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

