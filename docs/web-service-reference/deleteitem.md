---
title: DeleteItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItem
api_type:
- schema
ms.assetid: 055cdee8-3c7d-47db-9f27-740f4a674729
description: Элемент DeleteItem определяет запрос для удаления элемента из почтового ящика в хранилище Exchange.
ms.openlocfilehash: de64787750c88c8a47bb69daddc0a1d2ebe8bde9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762048"
---
# <a name="deleteitem"></a>DeleteItem

Элемент **DeleteItem** определяет запрос для удаления элемента из почтового ящика в хранилище Exchange. 
  
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
|**DeleteType** <br/> |Описывает, как удалить элемент. Этот атрибут является обязательным.  <br/> |
|**SendMeetingCancellations** <br/> |Описание, передается ли участникам удаления элемента календаря. Этот атрибут является обязательным, при удалении элементов календаря. Этот атрибут является необязательным, если удалить некалендарные элементы.  <br/> |
|**AffectedTaskOccurrences** <br/> |Описывает удалит ли [операция DeleteItem](deleteitem-operation.md)экземпляра задачи или шаблон задач. Этот атрибут является обязательным, при удалении задачи. Этот атрибут является необязательным при удалении элементов не задач.  <br/> |
|**SuppressReadReceipts** <br/> |Указывает, подавляются ли прочтении для удаленных элементов. Текстовое значение **true**, указывает, что прочтении подавляются. Значение **false** указывает, что прочтении отправляются отправителю. Этот атрибут является необязательным.  <br/> |
   
#### <a name="deletetype-attribute"></a>Атрибут DeleteType

|**Значение**|**Описание**|
|:-----|:-----|
|HardDelete  <br/> |Элемент окончательно удалить из хранилища.  <br/> |
|SoftDelete  <br/> |Перемещено в корзину Если корзина включена.  <br/> |
|MoveToDeletedItems  <br/> |Сообщение перемещено в папку «Удаленные».  <br/> |
   
#### <a name="sendmeetingcancellations-attribute"></a>Атрибут SendMeetingCancellations

|**Значение**|**Описание**|
|:-----|:-----|
|SendToNone  <br/> |Элемент календаря удаляется без отправки сообщения об отмене.  <br/> |
|SendOnlyToAll  <br/> |Удаленного элемента календаря и отмены сообщение отправляется всем участникам.  <br/> |
|SendToAllAndSaveCopy  <br/> |Удаленного элемента календаря и отмены сообщение отправляется всем участникам. Копия сообщения отмены сохраняется в папке «Отправленные».  <br/> |
   
#### <a name="affectedtaskoccurrences-attribute"></a>Атрибут AffectedTaskOccurrences

|**Значение**|**Описание**|
|:-----|:-----|
|AllOccurrences  <br/> |Запрос delete элемента удаляет главных задач и поэтому все повторяющиеся задачи, которые связаны с главной задачи.  <br/> |
|SpecifiedOccurrenceOnly  <br/> |Запрос delete элемента удаляет конкретных вхождений задачи.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Что ItemID](itemids.md) <br/> |Содержит массив элементов, элементы вхождений и повторяющиеся основные элементы для удаления из почтового ящика в хранилище Exchange. [DeleteItem операции](deleteitem-operation.md) можно выполнить на любой тип элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Параметры **MoveToDeletedItems** и **HardDelete** являются транзакций, это означает, что с на время завершения вызова веб-службы, базы данных переместить элемент папки «Удаленные» или окончательно удалить элемент из базы данных Exchange. Это поведение не зависит от MicrosoftExchange Server 2007 и Exchange Server 2010. 
  
Параметр **SoftDelete** работает по-разному для различных целевых версий Exchange. **SoftDelete** для Exchange Server 2007 немного задает для элемента, которое указывает, к базе данных Exchange, элемент перемещается в корзину папки в неопределенное время в будущем. **SoftDelete** для Exchange 2010 задает немедленное перемещение элемента в корзину. **SoftDelete** недоступно для удаления папки. Выполняет обход **SoftDelete** элементов и папок не возвращает результатов. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [DeleteItemResponse](deleteitemresponse.md)  
- [Операция DeleteItem](deleteitem-operation.md)

