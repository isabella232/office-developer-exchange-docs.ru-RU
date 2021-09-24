---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: Элемент DeleteItem определяет запрос на удаление элемента из почтового ящика в Exchange магазине.
ms.openlocfilehash: aa421de447126a22c1f01b3a0dc7498ff5b74a65
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528889"
---
# <a name="deleteitem"></a>DeleteItem

Элемент **DeleteItem** определяет запрос на удаление элемента из почтового ящика в Exchange магазине. 
  
```XML
<DeleteItem DeleteType="" SendMeetingCancellations="" AffectedTaskOccurrences="" SuppressReadReceipts="">
   <ItemIds/>
</DeleteItem>
```

 **DeleteItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**DeleteType** <br/> |Описывает, как удаляется элемент. Этот атрибут является обязательным.  <br/> |
|**SendMeetingCancellations** <br/> |Описывает, передается ли удаление элемента календаря участникам. Этот атрибут необходим при удалении элементов календаря. Этот атрибут необязателен, если элементы, не вписаные в календарь, удаляются.  <br/> |
|**AffectedTaskOccurrences** <br/> |Описывает, удаляется ли экземпляр задачи или мастер задачи операцией [DeleteItem.](deleteitem-operation.md) Этот атрибут необходим при удалении задач. Этот атрибут необязателен при удалении элементов, не в задачи.  <br/> |
|**SuppressReadReceipts** <br/> |Указывает, подавляются ли считывные квитанции для удаленного элемента. Текстовое значение **true** указывает на то, что квитанции чтения подавляются. Значение false **указывает** на то, что чеки чтения отправляются отправителю. Этот атрибут является необязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут DeleteType

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Элемент постоянно удаляется из магазина.  <br/> |
|SoftDelete  <br/> |Если элемент включен, элемент перемещается в контейнер.  <br/> |
|MoveToDeletedItems  <br/> |Сообщение перемещено в папку "Удаленные".  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Атрибут SendMeetingCancellations

|**Значение**|**Описание**|
|:-----|:-----|
|SendToNone  <br/> |Элемент календаря удаляется без отправки сообщения об отмене.  <br/> |
|SendOnlyToAll  <br/> |Элемент календаря удаляется, а всем участникам отправляется сообщение об отмене.  <br/> |
|SendToAllAndSaveCopy  <br/> |Элемент календаря удаляется, а всем участникам отправляется сообщение об отмене. Копия сообщения об отмене сохранена в папке Отправленные элементы.  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Атрибут AffectedTaskOccurrences

|**Значение**|**Описание**|
|:-----|:-----|
|AllOccurrences  <br/> |Запрос на удаление элемента удаляет главная задача и, следовательно, все повторяющиеся задачи, связанные с этой задачей.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Запрос на удаление элемента удаляет только определенные случаи задачи.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemIds](itemids.md) <br/> |Содержит массив элементов, элементов возникновения и повторяющихся мастер-элементов для удаления из почтового ящика в Exchange магазине. Операция [DeleteItem](deleteitem-operation.md) может выполняться на любом типе элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Параметры **MoveToDeletedItems** и **HardDelete** являются транзакциями, что означает, что к моменту завершения вызова веб-службы база данных переместила элемент в папку "Удаленные элементы" или окончательно удалила его из Exchange базы данных. Это поведение одинаково для MicrosoftExchange Server 2007 и Exchange Server 2010. 
  
Параметр **SoftDelete** работает по-разному для различных целевых версий Exchange. **SoftDelete** для Exchange 2007 задает элемент, который указывает в базу данных Exchange, что элемент будет перемещен в папку контейнера в неопределяемом времени в будущем. **SoftDelete** Exchange 2010 г. немедленно перемещает элемент в контейнер. **SoftDelete** не является вариантом удаления папок. **Поиск по обходу SoftDelete** для элементов и папок не возвращает результатов. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [DeleteItemResponse](deleteitemresponse.md)  
- [Операция DeleteItem](deleteitem-operation.md)

