---
title: максчанжесретурнед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: Элемент Максчанжесретурнед описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.
ms.openlocfilehash: caf96b6e95f2e63d0e544ead26fbea18cd637861
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460087"
---
# <a name="maxchangesreturned"></a>максчанжесретурнед

Элемент **максчанжесретурнед** описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации. 
  
[SyncFolderItems](syncfolderitems.md)
  
[максчанжесретурнед](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос на синхронизацию элементов в папке хранилища Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет целое число, которое описывает максимальное количество элементов, возвращаемых при каждом вызове синхронизации. Значение должно находиться в диапазоне от 1 до 512 включительно.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

