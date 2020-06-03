---
title: Actions (Рулеактионстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: Элемент Actions содержит список действий, связанных с правилами папки "Входящие".
ms.openlocfilehash: fbef3b69b1688d7c612af018d6a19f9ec1728066
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529681"
---
# <a name="actions-ruleactionstype"></a>Actions (Рулеактионстипе)

Элемент **Actions** содержит список действий, связанных с правилами папки "Входящие". 
  
```XML
<Actions>
   <AssignCategories/>
   <CopyToFolder/>
   <Delete/>
   <ForwardAsAttachmentToRecipients/>
   <ForwardToRecipients/>
   <MarkImportance/>
   <MarkAsRead/>
   <MoveToFolder/>
   <PermanentDelete/>
   <RedirectToRecipients/>
   <SendSMSAlertToRecipients/>
   <ServerReplyWithMessage/>
   <StopProcessingRules/>
</Actions>
```

 **рулеактионстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

[Ассигнкатегориес](assigncategories.md)  |  [CopyToFolder](copytofolder.md)  |  [Delete (удалить](delete.md)  |  ) [ФорвардасаттачменттореЦипиентс](forwardasattachmenttorecipients.md)  |  [ФорвардтореЦипиентс](forwardtorecipients.md)  |  [Маркимпортанце](markimportance.md)  |  [Маркасреад](markasread.md)  |  [MoveToFolder](movetofolder.md)  |  [Перманентделете](permanentdelete.md)  |  [RedirectToRecipients](redirecttorecipients.md)  |  [СендсмсалерттореЦипиентс](sendsmsalerttorecipients.md)  |  [Серверрепливисмессаже](serverreplywithmessage.md)  |  [StopProcessingRules](stopprocessingrules.md)
  
### <a name="parent-elements"></a>Родительские элементы

[Правило (RuleType)](rule-ruletype.md)
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

