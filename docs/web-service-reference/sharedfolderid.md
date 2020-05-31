---
title: шаредфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: Элемент Шаредфолдерид представляет идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом операции GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835477"
---
# <a name="sharedfolderid"></a>шаредфолдерид

Элемент **шаредфолдерид** представляет идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом [операции GetSharingFolder](getsharingfolder-operation.md) . 
  
```xml
<SharedFolderId/>
```

 **нонемптистрингтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |Определяет запрос на получение идентификатора локальной папки указанной общей папки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — это строка, представляющая идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом [операции GetSharingFolder](getsharingfolder-operation.md) . 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingFolder](getsharingfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

