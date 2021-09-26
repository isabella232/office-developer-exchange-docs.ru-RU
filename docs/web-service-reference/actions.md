---
title: Действия
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: Элемент Действия представляет набор действий, которые можно выполнить в сообщении при выполнении условий.
ms.openlocfilehash: 7f6608af5b8a9eb2772228a638fc42b9558f1e42
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546863"
---
# <a name="actions"></a>Действия

Элемент **Действия** представляет набор действий, которые можно выполнить в сообщении при выполнении условий. 
  
[Правило (RuleType)](rule-ruletype.md)
  
```XML
<Actions>
    <AssignCategories>
    <CopyToFolder>
    <Delete>
    <ForwardAsAttachmentToRecipients>
    <ForwardToRecipients>
    <MarkImportance>
    <MarkAsRead>
    <MoveToFolder>
    <PermanentDelete>
    <RedirectToRecipients>
    <SendSMSAlertToRecipients>
    <ServerReplyWithMessage>
    <StopProcessingRules>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AssignCategories](assigncategories.md) <br/> |Представляет категории, штампуемые в сообщениях электронной почты.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[удаление](delete.md); <br/> |Указывает, следует ли отправлять сообщения в папку "Удаленные элементы".  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Указывает адреса электронной почты, на которые сообщения должны быть переналожены в виде вложений.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Указывает адреса электронной почты, на которые должны отправляться сообщения.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Указывает значение, которое должно быть штампуется в сообщениях.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Указывает, должны ли сообщения быть помечены как чтение.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Указывает, следует ли постоянно удалять сообщения и не сохранить их в папке "Удаленные элементы".  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Указывает адреса электронной почты, на которые будут перенаправлены сообщения.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Указывает номера мобильных телефонов, на которые должно быть отправлено оповещение службы коротких сообщений (SMS).  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Указывает. ID сообщения шаблона, которое должно быть отправлено в качестве ответа на входящие сообщения.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Указывает, следует ли оценивать последующие правила.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет одно правило в почтовом ящике пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Conditions](conditions.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

