---
title: Задача
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: Элемент задачи представляет задачу в хранилище Exchange.
ms.openlocfilehash: 2c61fca6ac85290e34f1365b0cb9e841e1fe279f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840143"
---
# <a name="task"></a>Задача

Элемент **задачи** представляет задачу в хранилище Exchange. 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

**Тип задачи**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Subject](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объекты ответа.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Содержит сведения о состоянии уровень конфиденциальности сообщения элемента.  <br/> |
|[Body](body.md) <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах, элемента. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, к которому этот элемент является ее в ответ.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, является ли элемент был отправлен исходящие папке по умолчанию.  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет ли элемент еще не были отправлены.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемента для его сами себя.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, является ли элемент ранее еще был отправлен.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, были ли изменены элемента.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлен ли напоминания для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет число минут и только потом событие, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Строка отображения, который используется для содержимого в поле "Копия". Это составное строка всех получателей отображаемые имена «копия».  <br/> |
|[DisplayTo](displayto.md) <br/> |Строка отображения, который используется для содержимого в поле «Кому». Это составное строка всех для получателей отображаемые имена.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Язык и региональные параметры](culture.md) <br/> |Представляет язык и региональные параметры для заданного элемента в почтовом ящике.  <br/> |
|[ActualWork](actualwork.md) <br/> |Представляет фактическое время, затраченное на задачи.  <br/> |
|[AssignedTime](assignedtime.md) <br/> |Представляет время, когда задача назначена контакта.  <br/> |
|[BillingInformation](billinginformation.md) <br/> |Содержит сведения о задаче по выставлению счетов.  <br/> |
|[ChangeCount](changecount.md) <br/> |Указывает версию задачи.  <br/> |
|[Компании](companies.md) <br/> |Представляет коллекцию компании, связанные с контактом или задач.  <br/> |
|[CompleteDate](completedate.md) <br/> |Представляет дату, на котором выполняются.  <br/> |
|[Контакты](contacts-ex15websvcsotherref.md) <br/> |Содержит список контактов, связанных с задачей.  <br/> |
|[DelegationState](delegationstate.md) <br/> |Представляет состояние делегированные задачи.  <br/> |
|[Представитель](delegator.md) <br/> |Содержит имя сотрудника, назначена задача.  <br/> |
|[DueDate](duedate.md) <br/> |Представляет дату, когда срок выполнения элемента задачи.  <br/> |
|[IsAssignmentEditable](isassignmenteditable.md) <br/> |Указывает, является ли задача редактирования.  <br/> |
|[IsComplete](iscomplete.md) <br/> |Указывает, была выполнена ли задача или нет.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Указывает, является ли задача частью повторяющегося элемента. Этот элемент доступен только для чтения.  <br/> |
|[IsTeamTask](isteamtask.md) <br/> |Указывает, принадлежит ли задача группой.  <br/> |
|[Расстояние](mileage.md) <br/> |Представляет расстояние для элемента задачи.  <br/> |
|[Владелец](owner.md) <br/> |Представляет владельца задачи.  <br/> |
|[PercentComplete](percentcomplete.md) <br/> |Описание состояния завершения задания.  <br/> |
|[Повторение (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |Содержит данные о повторении для повторяющихся задач.  <br/> |
|[Дата начала](startdate.md) <br/> |Представляет дату начала элемента задачи.  <br/> |
|[Состояние](status.md) <br/> |Представляет состояние элемента задачи.  <br/> |
|[StatusDescription](statusdescription.md) <br/> |Содержит описание состояния задачи.  <br/> |
|[TotalWork](totalwork.md) <br/> |Содержит описание объем работы связан с элементом.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит правами клиент, построенный на параметры разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, является ли элемент связан с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления к отдельное свойство item/папки во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[Создание (ItemSync)](create-itemsync.md) <br/> |Определяет один элемент для создания в локальном хранилище клиента.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[Элементы](items.md) <br/> |Содержит массив элементов.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[Обновление (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание задач](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [Удаление задачи](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

