---
title: FindConversation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindConversation
api_type:
- schema
ms.assetid: 94b7083c-60cf-478b-a9af-a88f7acb30fb
description: Элемент FindConversation определяет запрос на поиск разговоров в почтовом ящике.
ms.openlocfilehash: e48e0d9fd71dac12fe6848031b2c056ea9a913ce
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59535172"
---
# <a name="findconversation"></a>FindConversation

Элемент **FindConversation** определяет запрос на поиск разговоров в почтовом ящике. 
  
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
|Traversal  <br/> |Определяет типы обхода под дерева. Этот атрибут является необязательным.  <br/> |
|ViewFilter  <br/> |Определяет фильтры представлений типов. Этот атрибут является необязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибута Traversal

****

|**Значение**|**Описание**|
|:-----|:-----|
|Shallow  <br/> |Указывает на неглубокий обход.  <br/> |
|Deep  <br/> |Указывает на глубокий обход.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Значения атрибута ViewFilter

****

|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Найдите все беседы.  <br/> |
|Помечено  <br/> |Поиск помеченных бесед.  <br/> |
|HasAttachment  <br/> |Поиск бесед с вложениями.  <br/> |
|ToOrCcMe  <br/> |Найдите беседы, адресованные или cc'd для меня.  <br/> |
|Unread  <br/> |Найдите непрочитанные беседы.  <br/> |
|TaskActive  <br/> |Поиск активных задач.  <br/> |
|TaskOverdue  <br/> |Поиск просроченных задач.  <br/> |
|TaskCompleted  <br/> |Поиск завершенных задач.  <br/> |
|NoClutter  <br/> |Только для внутреннего использования.  <br/> |
|Папка "Несрочные"  <br/> |Только для внутреннего использования.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[IndexedPageItemView](indexedpageitemview.md) <br/> |Описывает, как возвращается страница данных беседы.  <br/> |
|[SeekToConditionPageItemView](seektoconditionpageitemview.md) <br/> |Указывает условие, используемое для определения конца поиска, начального индекса поиска, максимального возврата записей и направлений поиска для поиска **FindItem** или **FindConversation.**  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет сортировку элементов в запросе операции [FindConversation.](findconversation-operation.md) Свойство **conversation:LastDeliveryTime** — это единственное свойство, которое поддерживается для сортировки при работе **с FindConversation.**  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Определяет папку для поиска разговоров.  <br/> |
|[MailboxScope](mailboxscope.md) <br/> |Указывает, должен ли поиск или извлечение для беседы охватывать основной почтовый ящик, архивный почтовый ящик или основной и архивный почтовый ящик.  <br/> |
|[QueryString (QueryStringType)](querystring-querystringtype.md) <br/> |Указывает строку запроса почтовых ящиков на основе синтаксиса расширенных запросов (AQS).  <br/> |
|[ConversationShape](conversationshape.md) <br/> |Определяет свойство, возвращаемую в ответе [операции FindConversation.](findconversation-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindConversation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

