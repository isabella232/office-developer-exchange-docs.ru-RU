---
title: Исключения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: Элемент исключения определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».
ms.openlocfilehash: b875b4dc0029bb9e0bc2bb50c41569fb72ef9268
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762417"
---
# <a name="exceptions"></a>Исключения

Элемент **исключения** определяет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие». 
  
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
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит категории, которые должны применяться к входящего сообщения в порядке для условие или исключение для применения.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Указывает строк, которые должны встречаться в теле входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indicaqtes строк, которые должны встречаться в заголовках входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Указывает строк, которые должны встречаться в параметр **ToRecipients** или **CcRecipients** свойства входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Указывает строк, которые должны встречаться в свойстве **из** входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Указывает строк, которые должны встречаться в тексте или теме входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Указывает строк, которые должны встречаться в теме входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Задает флаг, для которого действию задано значение, которое должно отображаться на входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Указывает адреса электронной почты, из которых необходимо отправить входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Представляет имена учетных записей электронной почты, из которых нужно были сводный в порядке для условие или исключение для применения входящих сообщений.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Указывает, будет ли входящих сообщений для получения вложений в порядке для условие или исключение для применения.  <br/> |
|[Важность](importance.md) <br/> |Указывает важность, записывается во входящих сообщениях в порядке для условие или исключение для применения.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Указывает, должен ли входящих сообщений запросов на утверждение в порядке для условие или исключение для применения.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Указывает, должен ли входящих сообщений автоматическая переадресация в порядке для условие или исключение для применения.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Указывает, должен ли входящих сообщений автоматических ответов в порядке для условие или исключение для применения.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Указывает, будет ли входящих сообщений должен быть зашифрован в порядке для условие или исключение для применения S/MIME.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Указывает, будет ли входящих сообщений должны быть приглашений на собрания в порядке для условие или исключение для применения.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Указывает, должен ли собрания ответы в порядке для условие или исключение для применения входящих сообщений.  <br/> |
|[IsNDR](isndr.md) <br/> |Указывает, должен ли входящих сообщений отчеты о недоставке (NDR) в порядке для условие или исключение для применения.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Указывает, входящих сообщений должен ли разрешение управляются (защищенные RMS) в порядке для условие или исключение для применения  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Указывает, должны ли прочитать поступлений в порядке для условие или исключение для применения входящих сообщений.  <br/> |
|[IsSigned](issigned.md) <br/> |Указывает, должен ли входящих сообщений в порядке для условие или исключение для применения подписью S/MIME.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Указывает, должен ли входящих сообщений сообщения голосовой почты в порядке для условие или исключение для применения.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Представляет элемент классы, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Представляет классификации сообщений, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Указывает, является ли владелец почтового ящика не должна быть в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Указывает, имеет ли владельца почтового ящика в свойство **CcRecipients** входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Указывает, является ли владелец почтового ящика должен быть только один в свойстве **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Указывает адреса электронной почты, которые должны входящих сообщений, отправленных в порядке для условие или исключение для применения.  <br/> |
|[SentToMe](senttome.md) <br/> |Указывает, имеет ли владельца почтового ящика в свойство **ToRecipients** входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Указывает, имеет ли владельца почтового ящика в **CcRecipients** или в **ToRecipients** свойство входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Указывает уровень конфиденциальности сообщения, которое необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Указывает диапазон дат, в течение которого нужно были получены в порядке для условие или исключение для применения входящих сообщений.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Указывает минимальный и максимальный размеры, которые должны быть входящих сообщений в порядке для условие или исключение для применения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Правило (RuleType)](rule-ruletype.md) <br/> |Содержит одно правило и представляет правило в почтовом ящике пользователя.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Предикаты правила используются как правила условий и исключений.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Условия](conditions.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

