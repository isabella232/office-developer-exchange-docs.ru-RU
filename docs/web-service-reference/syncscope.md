---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: Элемент SyncScope указывает ли только что элементов или элементы и сведения, папки, связанной возвращаются в ответ синхронизации.
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840130"
---
# <a name="syncscope"></a>SyncScope

Элемент **SyncScope** указывает ли только что элементов или элементы и сведения, папки, связанной возвращаются в ответ синхронизации. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Элемент, который определяет запрос для синхронизации элементов в папке хранилища Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/> / SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **SyncScope** . 
  
**Значения элементов SyncScope**

|**Значение**|**Описание**|
|:-----|:-----|
|NormalItems  <br/> |Указывает, что возвращаются только элементов в папке в ответ синхронизации.  <br/> |
|NormalAndAssociatedItems  <br/> |Указывает, что оба элементов в папке и сведений о папке связанного возвращаются в ответ синхронизации.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

