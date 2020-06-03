---
title: конверсатионактион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationAction
api_type:
- schema
ms.assetid: 9ecea41a-3860-4569-8e9b-284b451fc4e0
description: Элемент Конверсатионактион содержит одно действие, которое будет применено к одной беседе.
ms.openlocfilehash: cb7d874f787b105d5185749dfaf1e940d2411d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529254"
---
# <a name="conversationaction"></a>конверсатионактион

Элемент **конверсатионактион** содержит одно действие, которое будет применено к одной беседе. 
  
[ApplyConversationAction](applyconversationaction.md)
  
[конверсатионактионс](conversationactions.md)
  
[конверсатионактион](conversationaction.md)
  
```XML
<ConversationAction>
   <Action/>
   <ConversationId/>
   <ContextFolderId/>
   <ConversationLastSyncTime/>
   <ProcessRightAway/>
   <DestinationFolderId/>
   <Categories/>
   <EnableAlwaysDelete/>
   <IsRead/>
   <DeleteType/>
</ConversationAction>
```

 **конверсатионактионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Action (Конверсатионактионтипетипе)](action-conversationactiontypetype.md) <br/> |Содержит действие, которое необходимо выполнить для диалога, указанного с помощью элемента [ConversationId](conversationid.md) . Этот элемент должен присутствовать.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор диалога, который будет иметь действие, указанное элементом [Action (конверсатионактионтипетипе)](action-conversationactiontypetype.md) , примененным к элементам в беседе. Этот элемент должен присутствовать.  <br/> |
|[контекстфолдерид](contextfolderid.md) <br/> |Указывает папку, предназначенную для действий, в которых используются папки. Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.  <br/> |
|[конверсатионластсинктиме](conversationlastsynctime.md) <br/> |Содержит дату и время последней синхронизации беседы. Этот элемент должен присутствовать при попытке удалить все элементы в беседе, полученные до указанного времени.  <br/> |
|[процессригхтавай](processrightaway.md) <br/> |Указывает, отправляется ли ответ сразу после того, как действие начнет обработку на сервере или отправило ли ответ после завершения действия. Этот элемент должен присутствовать, чтобы ответ был асинхронно отправлен в запрошенное действие.  <br/> |
|[дестинатионфолдерид](destinationfolderid.md) <br/> |Указывает целевую папку для действий по копированию и перемещению.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, определяющих категории, к которым относятся элементы в беседе.  <br/> |
|[енаблеалвайсделете](enablealwaysdelete.md) <br/> |Указывает флаг, который включает удаление для всех новых элементов в беседе.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли Прочитано сообщение.  <br/> |
|[делететипе](deletetype.md) <br/> |Указывает, как удаляются элементы в беседе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактионс](conversationactions.md) <br/> |Содержит коллекцию бесед и действий, которые необходимо применить к ним.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**Текстовые значения элементов Конверсатионактион**

|**Значение**|**Описание**|
|:-----|:-----|
|алвайскатегоризе  <br/> |Всегда классифицировать беседу.  <br/> |
|алвайсделете  <br/> |Всегда удаляйте беседу.  <br/> |
|алвайсмове  <br/> |Всегда перемещайте беседу.  <br/> |
|Удаление  <br/> |Удаление беседы.  <br/> |
|Move  <br/> |Перемещение беседы.  <br/> |
|Copy  <br/> |Скопируйте беседу.  <br/> |
|сетреадстате  <br/> |Задание состояния чтения беседы.  <br/> |
|сетретентионполици  <br/> |Задайте политику хранения для беседы.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ApplyConversationAction](applyconversationaction-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

