---
title: Исключения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: Элемент Exceptions определяет исключения, которые представляют все доступные условия исключения правил для правила "Входящие".
ms.openlocfilehash: 5c92613aa871a200cf790e0709ba71280b226807
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524268"
---
# <a name="exceptions"></a>Исключения

Элемент **Exceptions** определяет исключения, которые представляют все доступные условия исключения правил для правила "Входящие". 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 **RulePredicatesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Содержит категории, которые необходимо применить к входящий сообщению для применения условия или исключения.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Указывает строки, которые должны отображаться в тексте входящих сообщений для применения условия или исключения.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indicaqtes the strings that must appear in the headers of incoming messages in order for the condition or exception to apply.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Указывает строки, которые должны отображаться в свойствах входящих сообщений **ToRecipients** или **CcRecipients** для применения условия или исключения.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Указывает строки, которые должны отображаться в свойстве **"От** входящих сообщений", чтобы применить условие или исключение.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Указывает строки, которые должны отображаться в теле или субъекте входящих сообщений для применения условия или исключения.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Указывает строки, которые должны отображаться в объекте входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Указывает флаг для значения действия, которое должно отображаться на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Указывает адреса электронной почты, с которых необходимо отправлять входящие сообщения для применения условия или исключения.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Представляет имена учетных записей электронной почты, из которых необходимо агрегировать входящие сообщения для применения условия или исключения.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Указывает, должны ли входящие сообщения иметь вложения для применения условия или исключения.  <br/> |
|[Importance](importance.md) <br/> |Указывает значение, которое штампуется для входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Указывает, должны ли входящие сообщения быть запросами на утверждение, чтобы применить условие или исключение.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Указывает, должны ли входящие сообщения быть автоматическими переададантами для применения условия или исключения.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Указывает, должны ли входящие сообщения быть автоматическими ответами для применения условия или исключения.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Указывает, должны ли входящие сообщения быть зашифрованы S/MIME для применения условия или исключения.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Указывает, должны ли входящие сообщения быть запросами на собрание, чтобы применить условие или исключение.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Указывает, должны ли входящие сообщения быть ответами на собрания, чтобы применить условие или исключение.  <br/> |
|[IsNDR](isndr.md) <br/> |Указывает, должны ли входящие сообщения быть отчетами о невывозе (NDRs) для применения условия или исключения.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Указывает, должны ли входящие сообщения контролироваться разрешениями (RMS защищены) для применения условия или исключения  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Указывает, должны ли входящие сообщения быть считывать квитанции для применения условия или исключения.  <br/> |
|[IsSigned](issigned.md) <br/> |Указывает, должны ли входящие сообщения подписываться на S/MIME для применения условия или исключения.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Указывает, должны ли входящие сообщения быть голосовой почтой для применения условия или исключения.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Представляет классы элементов, которые должны быть запечатаны на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Представляет классификации сообщений, которые необходимо штамповать на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Указывает, не должен ли владелец почтового ящика быть в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Указывает, должен ли владелец почтового ящика быть в свойстве **CcRecipients** входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Указывает, должен ли владелец почтового ящика быть единственным в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Указывает адреса электронной почты, на которые должны быть отправлены входящие сообщения, чтобы применить условие или исключение.  <br/> |
|[SentToMe](senttome.md) <br/> |Указывает, должен ли владелец почтового ящика быть в свойстве **ToRecipients** входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Указывает, должен ли владелец почтового ящика быть в свойстве **ToRecipients** или **CcRecipients** входящих сообщений, чтобы применить условие или исключение.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает чувствительность, которую необходимо штамповать на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Указывает диапазон дат, в пределах которого должны быть получены входящие сообщения, чтобы применить условие или исключение.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Указывает минимальные и максимальные размеры входящих сообщений для применения условия или исключения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правило (RuleType)](rule-ruletype.md) <br/> |Содержит одно правило и представляет правило в почтовом ящике пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Предикаты правила используются в качестве условий правила или исключений.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Conditions](conditions.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

