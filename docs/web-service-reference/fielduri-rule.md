---
title: FieldUri (Rule)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: Элемент FieldURI указывает URI в поле правил, которое вызвало ошибку проверки.
ms.openlocfilehash: c1390f6643614216fa86053368ba012cd0883ff7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513733"
---
# <a name="fielduri-rule"></a>FieldUri (Rule)

Элемент **FieldURI** указывает URI в поле правил, которое вызвало ошибку проверки. 
  
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
|[Ошибка](error.md) <br/> |Представляет одну ошибку проверки для определенного значения свойства правила, предикационного значения свойства или свойства действия.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для этого элемента ограничено одной из следующих строк:
  
- RuleId
    
- DisplayName
    
- Приоритет
    
- IsNotSupported
    
- Действия
    
- Condition:Categories
    
- Condition:ContainsBodyStrings
    
- Condition:ContainsHeaderStrings
    
- Condition:ContainsRecipientStrings
    
- Condition:ContainsSenderStrings
    
- Condition:ContainsSubjectOrBodyStrings
    
- Condition:ContainsSubjectStrings
    
- Condition:FlaggedForAction
    
- Condition:FromAddresses
    
- Condition:FromConnectedAccounts
    
- Condition:HasAttachments
    
- Condition:Importance
    
- Condition:IsApprovalRequest
    
- Condition:IsAutomaticForward
    
- Condition:IsAutomaticReply
    
- Condition:IsEncrypted
    
- Condition:IsMeetingRequest
    
- Condition:IsMeetingResponse
    
- Condition:IsNDR
    
- Condition:IsPermissionControlled
    
- Condition:IsReadReceipt
    
- Condition:IsSigned
    
- Condition:IsVoicemail
    
- Condition:ItemClasses
    
- Condition:MessageClassifications
    
- Condition:NotSentToMe
    
- Condition:SentCcMe
    
- Condition:SentOnlyToMe
    
- Condition:SentToAddresses
    
- Condition:SentToMe
    
- Condition:SentToOrCcMe
    
- Condition:Sensitivity
    
- Condition:WithinDateRange
    
- Condition:WithinSizeRange
    
- Исключение:Категории
    
- Исключение:ContainsBodyStrings
    
- Исключение:ContainsHeaderStrings
    
- Исключение:ContainsRecipientStrings
    
- Исключение:ContainsSenderStrings
    
- Исключение:ContainsSubjectOrBodyStrings
    
- Исключение:ContainsSubjectStrings
    
- Exception:FlaggedForAction
    
- Exception:FromAddresses
    
- Exception:FromConnectedAccounts
    
- Exception:HasAttachments
    
- Exception:Importance
    
- Исключение:IsApprovalRequest
    
- Исключение:IsAutomaticForward
    
- Исключение:IsAutomaticReply
    
- Исключение:IsEncrypted
    
- Исключение:IsMeetingRequest
    
- Исключение:IsMeetingResponse
    
- Исключение:IsNDR
    
- Исключение:IsPermissionControlled
    
- Исключение:IsReadReceipt
    
- Исключение:IsSigned
    
- Исключение:IsVoicemail
    
- Exception:ItemClasses
    
- Exception:MessageClassifications
    
- Исключение:NotSentToMe
    
- Exception:SentCcMe
    
- Exception:SentOnlyToMe
    
- Exception:SentToAddresses
    
- Exception:SentToMe
    
- Exception:SentToOrCcMe
    
- Исключение:Чувствительность
    
- Исключение:WithinDateRange
    
- Исключение:WithinSizeRange
    
- Action:AssignCategories
    
- Action:CopyToFolder
    
- Action:Delete
    
- Action:ForwardAsAttachmentToRecipients
    
- Action:ForwardToRecipients
    
- Action:MarkImportance
    
- Action:MarkAsRead
    
- Action:MoveToFolder
    
- Action:PermanentDelete
    
- Action:RedirectToRecipients
    
- Action:SendSMSAlertToRecipients
    
- Action:ServerReplyWithMessage
    
- Action:StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- Условия
    
- Исключения
    
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

