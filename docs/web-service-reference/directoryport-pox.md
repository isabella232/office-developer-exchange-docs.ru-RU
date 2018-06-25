---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: Элемент DirectoryPort определяет порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика имя службы (NSPI).
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762109"
---
# <a name="directoryport-pox"></a>DirectoryPort (POX)

Элемент **DirectoryPort** определяет порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика имя службы (NSPI). 
  
- [Автообнаружение (POX)](autodiscover-pox.md) 
- [Ответ (POX)](response-pox.md)  
- [Учетная запись (POX)](account-pox.md)  
- [Протокол (POX)](protocol-pox.md)  
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
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет порт, используемый для доступа к Exchange server.
  
## <a name="remarks"></a>Замечания

Элемент **DirectoryPort** используется только в том случае, когда элемент [Типа (POX)](type-pox.md) равняется EXCH или Выражение. 
  
## <a name="see-also"></a>См. также

- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

