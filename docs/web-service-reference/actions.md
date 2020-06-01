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
description: Элемент Actions представляет набор действий, которые могут быть выполнены над сообщением при выполнении условий.
ms.openlocfilehash: 2ac53778b583595fa8be07f2c5110a9e2df16eca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465067"
---
# <a name="actions"></a>Действия

Элемент **Actions** представляет набор действий, которые могут быть выполнены над сообщением при выполнении условий. 
  
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

 **рулеактионстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ассигнкатегориес](assigncategories.md) <br/> |Представляет категории, помеченные в сообщениях электронной почты.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[Удаление](delete.md) <br/> |Указывает, следует ли перемещать сообщения в папку "Удаленные".  <br/> |
|[форвардасаттачменттореЦипиентс](forwardasattachmenttorecipients.md) <br/> |Указывает адреса электронной почты, на которые будут пересылаться сообщения в виде вложений.  <br/> |
|[форвардтореЦипиентс](forwardtorecipients.md) <br/> |Указывает адреса электронной почты, на которые пересылаются сообщения.  <br/> |
|[маркимпортанце](markimportance.md) <br/> |Указывает важность, с которой будут отмечаться сообщения.  <br/> |
|[MarkAsRead](markasread.md) <br/> |Указывает, следует ли помечать сообщения как прочтенные.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.  <br/> |
|[перманентделете](permanentdelete.md) <br/> |Указывает, следует ли окончательно удалять сообщения и не сохранять их в папке "Удаленные".  <br/> |
|[RedirectToRecipients](redirecttorecipients.md) <br/> |Указывает адреса электронной почты, на которые перенаправляются сообщения.  <br/> |
|[сендсмсалерттореЦипиентс](sendsmsalerttorecipients.md) <br/> |Указывает номера мобильных телефонов, к которым отправляется оповещение в службе коротких сообщений (SMS).  <br/> |
|[серверрепливисмессаже](serverreplywithmessage.md) <br/> |Указывает. Идентификатор сообщения шаблона, отправляемого в качестве ответа на входящие сообщения.  <br/> |
|[StopProcessingRules](stopprocessingrules.md) <br/> |Указывает, следует ли оценивать последующие правила.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правило (RuleType)](rule-ruletype.md) <br/> |Представляет одно правило в почтовом ящике пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Conditions](conditions.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

