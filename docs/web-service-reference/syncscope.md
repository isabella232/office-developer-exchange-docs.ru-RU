---
title: синкскопе
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
description: Элемент Синкскопе указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой, а также сведения о них.
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463036"
---
# <a name="syncscope"></a>синкскопе

Элемент **синкскопе** указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой, а также сведения о них. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **синкфолдеритемсскопетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Элемент, определяющий запрос на синхронизацию элементов в папке хранилища Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/> /синкфолдеритемс  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **синкскопе** . 
  
**Значения элементов Синкскопе**

|**Значение**|**Описание**|
|:-----|:-----|
|нормалитемс  <br/> |Указывает, что в отклике синхронизации возвращаются только элементы в папке.  <br/> |
|нормаландассоЦиатедитемс  <br/> |Указывает, что оба элемента в папке и связанных с ней сведениями возвращаются в ответе синхронизации.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

