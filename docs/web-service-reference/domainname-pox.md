---
title: Имя_домена (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: Элемент имя_домена указывает домен пользователя.
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458427"
---
# <a name="domainname-pox"></a>Имя_домена (POX)

Элемент **имя_домена** указывает домен пользователя. 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md)  
- [Ответ (POX)](response-pox.md)  
- [Учетная запись (POX)](account-pox.md) 
- [Протокол (POX)](protocol-pox.md) 
- [Имя_домена (POX)](domainname-pox.md)
  
```xml
<DomainName/>
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

Текстовое значение указывает домен пользователя.
  
## <a name="remarks"></a>Примечания

Если значение не указано, по умолчанию используется проверка подлинности в формате имени участника-пользователя (UPN). Пример: \<Username\> @ \<Domain\> .
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

