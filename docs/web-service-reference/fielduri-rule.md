---
title: FieldUri (правила)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: Элемент FieldURI указывает URI в поле правило, вызвавшей ошибку проверки.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762527"
---
# <a name="fielduri-rule"></a>FieldUri (правила)

Элемент **FieldURI** указывает URI в поле правило, вызвавшей ошибку проверки. 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Error](error.md) <br/> |Представляет ошибку одной проверки на значение свойства определенное правило, значение свойства предиката или значение свойства действия.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для этого элемента есть только один из следующих строк:
  
- RuleId
    
- DisplayName
    
- Priority
    
- IsNotSupported
    
- Действия
    
- Условие: категории
    
- Условие: ContainsBodyStrings
    
- Условие: ContainsHeaderStrings
    
- Условие: ContainsRecipientStrings
    
- Условие: ContainsSenderStrings
    
- Условие: ContainsSubjectOrBodyStrings
    
- Условие: ContainsSubjectStrings
    
- Условие: FlaggedForAction
    
- Условие: FromAddresses
    
- Условие: FromConnectedAccounts
    
- Условие: HasAttachments
    
- Условие: важность
    
- Условие: IsApprovalRequest
    
- Условие: IsAutomaticForward
    
- Условие: IsAutomaticReply
    
- Условие: IsEncrypted
    
- Условие: IsMeetingRequest
    
- Условие: IsMeetingResponse
    
- Условие: IsNDR
    
- Условие: IsPermissionControlled
    
- Условие: IsReadReceipt
    
- Условие: IsSigned
    
- Условие: IsVoicemail
    
- Условие: ItemClasses
    
- Условие: MessageClassifications
    
- Условие: NotSentToMe
    
- Условие: SentCcMe
    
- Условие: SentOnlyToMe
    
- Условие: SentToAddresses
    
- Условие: SentToMe
    
- Условие: SentToOrCcMe
    
- Условие: уровень конфиденциальности сообщения
    
- Условие: WithinDateRange
    
- Условие: WithinSizeRange
    
- Исключение: категории
    
- Исключение: ContainsBodyStrings
    
- Исключение: ContainsHeaderStrings
    
- Исключение: ContainsRecipientStrings
    
- Исключение: ContainsSenderStrings
    
- Исключение: ContainsSubjectOrBodyStrings
    
- Исключение: ContainsSubjectStrings
    
- Исключение: FlaggedForAction
    
- Исключение: FromAddresses
    
- Исключение: FromConnectedAccounts
    
- Исключение: HasAttachments
    
- Исключение: важность
    
- Исключение: IsApprovalRequest
    
- Исключение: IsAutomaticForward
    
- Исключение: IsAutomaticReply
    
- Исключение: IsEncrypted
    
- Исключение: IsMeetingRequest
    
- Исключение: IsMeetingResponse
    
- Исключение: IsNDR
    
- Исключение: IsPermissionControlled
    
- Исключение: IsReadReceipt
    
- Исключение: IsSigned
    
- Исключение: IsVoicemail
    
- Исключение: ItemClasses
    
- Исключение: MessageClassifications
    
- Исключение: NotSentToMe
    
- Исключение: SentCcMe
    
- Исключение: SentOnlyToMe
    
- Исключение: SentToAddresses
    
- Исключение: SentToMe
    
- Исключение: SentToOrCcMe
    
- Исключение: уровень конфиденциальности сообщения
    
- Исключение: WithinDateRange
    
- Исключение: WithinSizeRange
    
- Действие: AssignCategories
    
- Действие: CopyToFolder
    
- Действие: удаление
    
- Действие: ForwardAsAttachmentToRecipients
    
- Действие: ForwardToRecipients
    
- Действие: MarkImportance
    
- Действие: MarkAsRead
    
- Действие: MoveToFolder
    
- Действие: PermanentDelete
    
- Действие: RedirectToRecipients
    
- Действие: SendSMSAlertToRecipients
    
- Действие: ServerReplyWithMessage
    
- Действие: StopProcessingRules
    
- Свойства IsEnabled
    
- IsInError
    
- Условия
    
- Исключения
    
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

