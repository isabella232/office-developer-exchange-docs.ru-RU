---
title: Действия
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Actions
api_type:
- schema
ms.assetid: c5aa96b1-2d8b-422f-8c2f-f118572ab23f
description: Элемент Actions представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.
ms.openlocfilehash: 093d2f28135c6077b6cea488591573af0182934b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761330"
---
# <a name="actions"></a>Действия

Элемент **Actions** представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены. 
  
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
|[AssignCategories](assigncategories.md) <br/> |Представляет категории, которые имеют на сообщения электронной почты.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определение идентификатора к папке, где будет скопировано элементов электронной почты.  <br/> |
|[удаление](delete.md); <br/> |Указывает, будет ли сообщений перемещаются в папку «Удаленные».  <br/> |
|[ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) <br/> |Указывает адреса электронной почты, к которым сообщения, пересылаемые в виде вложений.  <br/> |
|[ForwardToRecipients](forwardtorecipients.md) <br/> |Указывает адреса электронной почты, к которым сообщения, для перенаправления.  <br/> |
|[MarkImportance](markimportance.md) <br/> |Задает важность, ставится отметка в сообщениях.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Указывает, будет ли сообщений помечена как прочтенные.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определение идентификатора к папке, где планируется переместить сообщения электронной почты.  <br/> |
|[PermanentDelete](permanentdelete.md) <br/> |Указывает, являются ли сообщения для окончательного удаления и не сохраняются в папку «Удаленные».  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Указывает адреса электронной почты, к которым должны перенаправляться сообщения.  <br/> |
|[SendSMSAlertToRecipients](sendsmsalerttorecipients.md) <br/> |Указывает, номера мобильного телефона, к которым будет отправляться уведомление службы коротких сообщений (SMS).  <br/> |
|[ServerReplyWithMessage](serverreplywithmessage.md) <br/> |Указывает. Идентификатор шаблона сообщения, которые отправляются в виде ответа на входящие сообщения.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Указывает, являются ли последующих правил для оценки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет одно правило в почтовом ящике пользователя.  <br/> |
   
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
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Условия](conditions.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

