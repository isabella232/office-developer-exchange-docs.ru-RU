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
# <a name="actions-ruleactionstype"></a><span data-ttu-id="1afbd-103">Actions (Рулеактионстипе)</span><span class="sxs-lookup"><span data-stu-id="1afbd-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="1afbd-104">Элемент **Actions** содержит список действий, связанных с правилами папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="1afbd-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="1afbd-105">**рулеактионстипе**</span><span class="sxs-lookup"><span data-stu-id="1afbd-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1afbd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1afbd-106">Attributes and elements</span></span>

<span data-ttu-id="1afbd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1afbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1afbd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1afbd-108">Attributes</span></span>

<span data-ttu-id="1afbd-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1afbd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1afbd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1afbd-110">Child elements</span></span>

<span data-ttu-id="1afbd-111">[Ассигнкатегориес](assigncategories.md)  |  [CopyToFolder](copytofolder.md)  |  [Delete (удалить](delete.md)  |  ) [ФорвардасаттачменттореЦипиентс](forwardasattachmenttorecipients.md)  |  [ФорвардтореЦипиентс](forwardtorecipients.md)  |  [Маркимпортанце](markimportance.md)  |  [Маркасреад](markasread.md)  |  [MoveToFolder](movetofolder.md)  |  [Перманентделете](permanentdelete.md)  |  [RedirectToRecipients](redirecttorecipients.md)  |  [СендсмсалерттореЦипиентс](sendsmsalerttorecipients.md)  |  [Серверрепливисмессаже](serverreplywithmessage.md)  |  [StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="1afbd-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1afbd-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1afbd-112">Parent elements</span></span>

[<span data-ttu-id="1afbd-113">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="1afbd-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="1afbd-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="1afbd-114">Remarks</span></span>

<span data-ttu-id="1afbd-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1afbd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1afbd-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1afbd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1afbd-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1afbd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1afbd-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1afbd-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1afbd-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1afbd-119">Schema name</span></span>  <br/> |<span data-ttu-id="1afbd-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1afbd-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1afbd-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1afbd-121">Validation file</span></span>  <br/> |<span data-ttu-id="1afbd-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1afbd-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1afbd-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1afbd-123">Can be empty</span></span>  <br/> |<span data-ttu-id="1afbd-124">false</span><span class="sxs-lookup"><span data-stu-id="1afbd-124">false</span></span>  <br/> |
   

