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
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466124"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingFolder](getsharingfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

