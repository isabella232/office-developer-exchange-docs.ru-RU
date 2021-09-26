---
title: ConnectionFailureCause
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionFailureCause
api_type:
- schema
ms.assetid: d2160c8a-015c-4964-b7f7-93478764a173
description: Элемент ConnectionFailureCause указывает причину отключения от телефонного звонка.
ms.openlocfilehash: de2f06ae89577b0141b8555f98dba1671a228d45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543536"
---
# <a name="connectionfailurecause"></a>ConnectionFailureCause

Элемент **ConnectionFailureCause** указывает причину отключения от телефонного звонка. 
  
```xml
<ConnectionFailureCause>None or UserBusy or NoAnswer or Unavailable or Other</ConnectionFailureCause>
```

 **ConnectionFailureCauseType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Указывает сведения о состоянии для телефонного звонка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **ConnectionFailureCause.** 
  
**Значения элементов ConnectionFailureCause**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Состояние вызова не отключено или причина отключения неизвестна.  <br/> |
|UserBusy  <br/> |Вызванная линия участника была занята.  <br/> |
|NoAnswer  <br/> |Вызванная сторона не ответила.  <br/> |
|Недоступно  <br/> |Номер вызванной стороны не был доступен.  <br/> |
|Другие  <br/> |Catch-all по другим причинам отключения.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

