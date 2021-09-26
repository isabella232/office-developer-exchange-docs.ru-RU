---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: Элемент DirectoryPort указывает порт, используемый для подключения к каталогу, когда используется протокол интерфейса поставщика служб имени (NSPI).
ms.openlocfilehash: 223e82840628e19896bde196d7467622a2ad5002
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543333"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

Элемент **DirectoryPort** указывает порт, используемый для подключения к каталогу, когда используется протокол интерфейса поставщика служб имени (NSPI). 
  
- [AutoDiscover (POX)](autodiscover-pox.md) 
- [Response (POX)](response-pox.md)  
- [Account (POX)](account-pox.md)  
- [Protocol (POX)](protocol-pox.md)  
- [DirectoryPort (POX)](directoryport-pox.md)
  
```xml
<DirectoryPort/>
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

Текстовое значение представляет порт, используемый для доступа к Exchange серверу.
  
## <a name="remarks"></a>Заметки

Элемент **DirectoryPort** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен EXCH или EXPR. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

