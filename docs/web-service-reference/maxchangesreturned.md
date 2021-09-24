---
title: MaxChangesReturned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: Элемент MaxChangesReturned описывает максимальное количество изменений, которые могут быть возвращены в ответ на синхронизацию.
ms.openlocfilehash: 8169e1a87ed22b68e5115cd7eaaa1084e44e8f33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523938"
---
# <a name="maxchangesreturned"></a>MaxChangesReturned

Элемент **MaxChangesReturned** описывает максимальное количество изменений, которые могут быть возвращены в ответ на синхронизацию. 
  
[SyncFolderItems](syncfolderitems.md)
  
[MaxChangesReturned](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Определяет запрос на синхронизацию элементов в Exchange папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет собой целый ряд, который описывает максимальное количество элементов, возвращаемых в одном вызове синхронизации. Значение должно быть от 1 до 512 включительно.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

