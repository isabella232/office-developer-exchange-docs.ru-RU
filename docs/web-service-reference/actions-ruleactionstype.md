---
title: Действия (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: Элемент Actions содержит список действий, связанных с помощью правил папки "Входящие".
ms.openlocfilehash: 8ed8095ca8b41e037c2c0dad319c9c4ab99ed2bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761419"
---
# <a name="actions-ruleactionstype"></a><span data-ttu-id="6b143-103">Действия (RuleActionsType)</span><span class="sxs-lookup"><span data-stu-id="6b143-103">Actions (RuleActionsType)</span></span>

<span data-ttu-id="6b143-104">Элемент **Actions** содержит список действий, связанных с помощью правил папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6b143-104">The **Actions** element contains a list of actions associated with Inbox rules.</span></span> 
  
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

 <span data-ttu-id="6b143-105">**RuleActionsType**</span><span class="sxs-lookup"><span data-stu-id="6b143-105">**RuleActionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b143-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b143-106">Attributes and elements</span></span>

<span data-ttu-id="6b143-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6b143-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b143-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b143-108">Attributes</span></span>

<span data-ttu-id="6b143-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b143-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b143-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b143-110">Child elements</span></span>

<span data-ttu-id="6b143-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Удаление](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead ](markasread.md)  |  [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md)  |  [ StopProcessingRules](stopprocessingrules.md)</span><span class="sxs-lookup"><span data-stu-id="6b143-111">[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Delete](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead](markasread.md) | [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md) | [StopProcessingRules](stopprocessingrules.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b143-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b143-112">Parent elements</span></span>

[<span data-ttu-id="6b143-113">Правило (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6b143-113">Rule (RuleType)</span></span>](rule-ruletype.md)
  
## <a name="remarks"></a><span data-ttu-id="6b143-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="6b143-114">Remarks</span></span>

<span data-ttu-id="6b143-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b143-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b143-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b143-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b143-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b143-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b143-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b143-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b143-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b143-119">Schema name</span></span>  <br/> |<span data-ttu-id="6b143-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6b143-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="6b143-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b143-121">Validation file</span></span>  <br/> |<span data-ttu-id="6b143-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b143-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b143-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b143-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6b143-124">Нет</span><span class="sxs-lookup"><span data-stu-id="6b143-124">false</span></span>  <br/> |
   

