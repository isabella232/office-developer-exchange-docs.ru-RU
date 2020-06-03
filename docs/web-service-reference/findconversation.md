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
description: Элемент FindConversation определяет запрос на поиск бесед в почтовом ящике.
ms.openlocfilehash: 98d692132ed9375d981c95d24600b0e2c4b1d8c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462649"
---
# <a name="findconversation"></a>FindConversation

Элемент **FindConversation** определяет запрос на поиск бесед в почтовом ящике. 
  
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

 **финдконверсатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

****

|**Атрибут**|**Описание**|
|:-----|:-----|
|Обход  <br/> |Определяет типы обхода вложенного дерева. Этот атрибут является необязательным.  <br/> |
|виевфилтер  <br/> |Определяет фильтры представления типов. Этот атрибут является необязательным.  <br/> |
   
#### <a name="traversal-attribute-values"></a>Значения атрибутов обхода

****

|**Значение**|**Описание**|
|:-----|:-----|
|Поверхност  <br/> |Обозначает неполную обходов.  <br/> |
|Углублен  <br/> |Указывает на глубокий обход.  <br/> |
   
#### <a name="viewfilter-attribute-values"></a>Значения атрибутов Виевфилтер

****

|**Значение**|**Описание**|
|:-----|:-----|
|Все  <br/> |Поиск всех бесед.  <br/> |
|Отмеченные  <br/> |Поиск помеченных бесед.  <br/> |
|HasAttachment  <br/> |Поиск бесед с вложениями.  <br/> |
|турккме  <br/> |Поиск бесед, адресованных или получателей CC.  <br/> |
|Unread  <br/> |Поиск непрочитанных бесед.  <br/> |
|таскактиве  <br/> |Поиск активных задач.  <br/> |
|тасковердуе  <br/> |Поиск просроченных задач.  <br/> |
|тасккомплетед  <br/> |Поиск завершенных задач.  <br/> |
|Функция "несрочные"  <br/> |Только для внутреннего использования.  <br/> |
|Папка "Несрочные"  <br/> |Только для внутреннего использования.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[индекседпажеитемвиев](indexedpageitemview.md) <br/> |Описывает, как возвращаются сведения о страничной беседе.  <br/> |
|[сиктокондитионпажеитемвиев](seektoconditionpageitemview.md) <br/> |Задает условие, используемое для определения конца поиска, начального индекса поиска, максимальных возвращаемых значений и направления поиска для поиска **FindItem** или **FindConversation** .  <br/> |
|[SortOrder](sortorder.md) <br/> |Определяет порядок сортировки элементов в запросе [операции FindConversation](findconversation-operation.md) . Свойство **CONVERSATION: ластделиверитиме** — единственное свойство, которое поддерживается для сортировки при использовании операции **FindConversation** .  <br/> |
|[ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) <br/> |Определяет папку для поиска обсуждений.  <br/> |
|[маилбоксскопе](mailboxscope.md) <br/> |Указывает, следует ли выполнять поиск или выборку для беседы: в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.  <br/> |
|[Строка запроса (Куеристрингтипе)](querystring-querystringtype.md) <br/> |Указывает строку запроса к почтовому ящику на основе расширенного синтаксиса запросов (AQS).  <br/> |
|[конверсатионшапе](conversationshape.md) <br/> |Определяет значение свойства, возвращаемого в ответе [операции FindConversation](findconversation-operation.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindConversation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

