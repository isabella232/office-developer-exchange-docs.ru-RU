---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: Элемент FindConversation определяет запрос на поиск бесед в почтовый ящик.
ms.openlocfilehash: 990e15f468f836d51977329c524acb439014da95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762555"
---
# <a name="findconversation"></a>FindConversation

Элемент **FindConversation** определяет запрос на поиск бесед в почтовый ящик. 
  
[FindConversation](findconversation.md)
  
```XML
<FindConversation Traversal="" ViewFilter="">
   <IndexedPageItemView/>
   <SeekToConditionPageItemView/>
   <SortOrder/>
   <ParentFolderId/>
   <MailboxScope/>
   <QueryString/>
   <ConversationShape/>
</FindConversation>
```

 **FindConversationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

****

|**Атрибут**|**Описание**|
|:-----|:-----|
|Обход  <br/> |Определяет типы поддерева обхода. Этот атрибут является необязательным.  <br/> |
|ViewFilter  <br/> |Определяет типы фильтры представления. Этот атрибут является необязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

****

|**Значение**|**Описание**|
|:-----|:-----|
|Неполная  <br/> |Указывает частичного обхода.  <br/> |
|Глубокое  <br/> |Указывает глубину обхода.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Значения атрибутов ViewFilter

****

|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Поиск всех бесед.  <br/> |
|Отмеченные  <br/> |Поиск отмеченного бесед.  <br/> |
|HasAttachment  <br/> |Поиск бесед с вложениями.  <br/> |
|ToOrCcMe  <br/> |Найдите адресованное беседы или «копия» будет мне.  <br/> |
|Unread  <br/> |Поиск непрочитанных бесед.  <br/> |
|TaskActive  <br/> |Поиск активных задач.  <br/> |
|TaskOverdue  <br/> |Найдите просроченные задачи.  <br/> |
|TaskCompleted  <br/> |Найдите завершенные задачи.  <br/> |
|NoClutter  <br/> |Только для внутреннего использования.  <br/> |
|Засорение  <br/> |Только для внутреннего использования.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Описывает как выгружаемый беседы возвращаются данные.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Указывает условие, используемый для идентификации в конце поиска, начальный индекс поиска, максимальное записей для возвращения и указания поиска для поиска **FindItem** или **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет порядок сортировки элементов в [FindConversation операции](findconversation-operation.md) запроса. Свойство **Беседы: LastDeliveryTime** — это единственный параметр, который поддерживается для сортировки при использовании операции **FindConversation** .  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Указывает папку для поиска бесед.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Разрешение поиска или выборки для беседы должны охватывать основной почтовый ящик, архивного почтового ящика или обеих основной и архивировать почтового ящика.  <br/> |
|[Строка запроса (QueryStringType)](querystring-querystringtype.md) <br/> |Указывает строку запроса почтовых ящиков на основе на расширенный синтаксис запроса (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Определяет свойство, задайте для возврата в ответ на [операцию FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindConversation Operation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

