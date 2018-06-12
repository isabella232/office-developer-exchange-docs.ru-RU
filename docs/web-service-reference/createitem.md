---
title: CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: c3707feb-3fd4-4b8a-a68f-2abadd455163
description: Элемент CreateItem определяет запрос для создания элемента в хранилище Exchange.
ms.openlocfilehash: bb5cddd5ea4fa1b73c424275a0b0219ce3e189e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761898"
---
# <a name="createitem"></a>CreateItem

Элемент **CreateItem** определяет запрос для создания элемента в хранилище Exchange. 
  
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

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MessageDisposition** <br/> |Описывает, как будут обрабатываться элемент после его создания. Атрибут является обязательным для сообщений электронной почты. Этот атрибут применим только к сообщениям электронной почты.  <br/> |
|**SendMeetingInvitations** <br/> |Описывает порядок обработки приглашений на собрание после их создания. Этот атрибут является обязательным для элементов календаря.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Атрибут MessageDisposition

|**Значение**|**Описание**|
|:-----|:-----|
|SaveOnly  <br/> |Элемент сообщение сохраняется в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) . Сообщения могут быть отправлены более поздней версии с помощью [операции SendItem](senditem-operation.md). Идентификатор элемента возвращаемого в ответе. Идентификаторы элементов не возвращаются для любых типов элементов, за исключением элементы сообщения. Этот компонент включает объекты ответа.  <br/> |
|SendOnly  <br/> |Элемент отправляется, но копия не сохраняется в папке «Отправленные». Идентификатор элемента не возвращается в ответе.  <br/> > [!NOTE]> **CreateItem** не поддерживает делегированный доступ, когда используется параметр SendOnly, так как этот параметр нельзя использовать папку назначения. Обходным путем является создание элемента, получить идентификатор элемента и затем использовать операцию SendItem для отправки элемента.           |
|SendAndSaveCopy  <br/> |Элемент отправляется и копия сохраняется в папке, которая определена в элементе [SavedItemFolderId](saveditemfolderid.md) . Идентификатор элемента не возвращается в ответе.  <br/> > [!NOTE]> Приглашения на собрания не сохраняются в папке, заданной свойством [SavedItemFolderId](saveditemfolderid.md) . Для функции календаря, только сохранения в свойстве **SavedItemFolderId** можно указать расположение элементов календаря. Вы не можете определять, приглашения на собрание элемент был сохранен. Связанных элементов календаря, копируются и сохраняются в папке, заданной свойством **SavedItemFolderId** .           |
   
#### <a name="sendmeetinginvitations-attribute"></a>Атрибут SendMeetingInvitations

|**Значение**|**Описание**|
|:-----|:-----|
|SendToNone  <br/> |Если элемент имеет приглашения на собрание, сохраняемый в виде элемента календаря, но не отправляются.  <br/> |
|SendOnlyToAll  <br/> |Запрос на собрание отправляется всех участников, но не сохраняются в папке «Отправленные».  <br/> |
|SendToAllAndSaveCopy  <br/> |Всем участникам отправляется запрос на собрание и копия сохраняется в папке, которая определена в элементе [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет целевой папке, где можно создать новый элемент. Если атрибут **MessageDisposition** SendOnly, созданного сообщения будут отправляться только. Сообщение не следует помещать в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
|[Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, указанной с помощью элемента [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[CreateItemResponse](createitemresponse.md)
  
[CreateItem Operation](createitem-operation.md)
  
 **CreateItemType**


[Создание сообщения электронной почты](http://msdn.microsoft.com/library/05bfb83c-2866-427d-a9fe-14ba3cb02793%28Office.15%29.aspx)
  
[Создание контактов (веб-служб Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Создание задач](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Создание встреч](http://msdn.microsoft.com/library/2385391e-c9e7-4d45-b803-c4ff94d5c94e%28Office.15%29.aspx)

