---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: Элемент CreateItem определяет запрос на создание элемента в Exchange магазине.
ms.openlocfilehash: 7276b88bd3b90edc68d7ac8fd4a7646324eadb61
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526500"
---
# <a name="createitem"></a>CreateItem

Элемент **CreateItem** определяет запрос на создание элемента в Exchange магазине. 
  
```xml
<CreateItem MessageDisposition="" SendMeetingInvitations="">
   <SavedItemFolderId/>
   <Items/>
</CreateItem>
```

**CreateItemType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|Атрибут|Описание|
|:-----|:-----|
|**MessageDisposition** <br/> |Описывает, как будет обрабатываться элемент после его создания. Атрибут необходим для сообщений электронной почты. Этот атрибут применим только к сообщениям электронной почты.  <br/> |
|**SendMeetingInvitations** <br/> |Описывает обработку запросов собраний после их создания. Этот атрибут необходим для элементов календаря.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Атрибут MessageDisposition

|Значение|Описание|
|:-----|:-----|
|SaveOnly  <br/> |Элемент сообщения сохранен в папке, указанной элементом [SavedItemFolderId.](saveditemfolderid.md) Сообщения можно отправлять позже с помощью [операции SendItem.](senditem-operation.md) Идентификатор элемента возвращается в ответе. Идентификаторы элементов не возвращаются для любых типов элементов, за исключением элементов сообщений. Это включает объекты отклика.  <br/> |
|SendOnly  <br/> |Элемент отправляется, но копия не сохранена в папке Отправленные элементы. Идентификатор элемента не возвращается в ответе.<br/><br/>**ПРИМЕЧАНИЕ.** **CreateItem** не поддерживает доступ к делегатам, когда используется параметр SendOnly, так как папка назначения не может быть указана с помощью этого параметра. Обходным решением является создание элемента, создание идентификатора элемента, а затем использование операции SendItem для отправки элемента.           |
|SendAndSaveCopy  <br/> |Элемент отправляется, а копия сохранена в папке, которая идентифицирована элементом [SavedItemFolderId.](saveditemfolderid.md) Идентификатор элемента не возвращается в ответе.<br/><br/>**ПРИМЕЧАНИЕ.** Запросы на собрания не сохраняются в папке, которая определена [свойством SavedItemFolderId.](saveditemfolderid.md) Для календаря свойство **SavedItemFolderId** может задать только расположение сохранения элементов календаря. Невозможно контролировать, где сохранен элемент запроса на собрание. Только связанные элементы календаря копируются и сохраняются в папке, идентифицированной **свойством SavedItemFolderId.**           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Атрибут SendMeetingInvitations

|Значение|Описание|
|:-----|:-----|
|SendToNone  <br/> |Если элемент является запросом на собрание, он сохранен как элемент календаря, но не отправлен.  <br/> |
|SendOnlyToAll  <br/> |Запрос на собрание отправляется всем участникам, но не сохранен в папке Отправленные элементы.  <br/> |
|SendToAllAndSaveCopy  <br/> |Запрос на собрание отправляется всем участникам, а копия сохранена в папке, идентифицированной элементом [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|Элемент|Описание|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет целевую папку, в которой можно создать новый элемент. Если атрибут **MessageDisposition** настроен на SendOnly, созданное сообщение будет отправлено только. Сообщение не будет помещаться в папку, идентифицированную элементом [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, которая определена элементом [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [CreateItemResponse](createitemresponse.md)  
- [Операция CreateItem](createitem-operation.md)
- [Создание сообщений электронной почты](https://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx) 
- [Создание контактов (Exchange веб-служб)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)  
- [Создание задач](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [Создание встреч](https://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

