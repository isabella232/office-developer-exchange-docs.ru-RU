---
title: Директорипорт (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: Элемент Директорипорт указывает порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика услуг имен (NSPI).
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462089"
---
# <a name="directoryport-pox"></a>Директорипорт (POX)

Элемент **директорипорт** указывает порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика услуг имен (NSPI). 
  
- [Служба автообнаружения (POX)](autodiscover-pox.md) 
- [Ответ (POX)](response-pox.md)  
- [Учетная запись (POX)](account-pox.md)  
- [Протокол (POX)](protocol-pox.md)  
- [Директорипорт (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
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

Текстовое значение представляет порт, используемый для доступа к серверу Exchange Server.
  
## <a name="remarks"></a>Примечания

Элемент **директорипорт** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен "сумме" или "expr". 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

