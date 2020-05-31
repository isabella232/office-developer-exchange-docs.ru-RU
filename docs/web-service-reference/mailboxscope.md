---
title: маилбоксскопе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: Элемент Маилбоксскопе указывает, следует ли выполнять поиск или получение для беседы в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834293"
---
# <a name="mailboxscope"></a><span data-ttu-id="3ef16-103">маилбоксскопе</span><span class="sxs-lookup"><span data-stu-id="3ef16-103">MailboxScope</span></span>

<span data-ttu-id="3ef16-104">Элемент **маилбоксскопе** указывает, следует ли выполнять поиск или получение для беседы в основном почтовом ящике, архивном почтовом ящике или основном и архивном почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3ef16-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="3ef16-105">**маилбокссеарчлокатионтипе**</span><span class="sxs-lookup"><span data-stu-id="3ef16-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3ef16-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3ef16-106">Attributes and elements</span></span>

<span data-ttu-id="3ef16-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3ef16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ef16-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3ef16-108">Attributes</span></span>

<span data-ttu-id="3ef16-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3ef16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ef16-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3ef16-110">Child elements</span></span>

<span data-ttu-id="3ef16-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="3ef16-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3ef16-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3ef16-112">Parent elements</span></span>

<span data-ttu-id="3ef16-113">[FindConversation](findconversation.md) | Беседа с FindConversation[GetConversationItems](getconversationitems.md) | [(конверсатионтипе)](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="3ef16-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3ef16-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3ef16-114">Text value</span></span>

<span data-ttu-id="3ef16-115">Текстовое значение элемента **маилбоксскопе** является областью для поиска или получение элементов в беседе в основных почтовых ящиках, архивных почтовых ящиках или как в основном, так и в архивных почтовых ящиках.</span><span class="sxs-lookup"><span data-stu-id="3ef16-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="3ef16-116">Текстовое значение **PrimaryOnly** указывает область, предназначенную для основного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ef16-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="3ef16-117">Текстовое значение **ArchiveOnly** указывает область, предназначенную для архивного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="3ef16-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="3ef16-118">Текстовое значение **ALL** указывает область, которая предназначена как для основного почтового ящика, так и для архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3ef16-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3ef16-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="3ef16-119">Remarks</span></span>

<span data-ttu-id="3ef16-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3ef16-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3ef16-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ef16-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ef16-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3ef16-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ef16-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3ef16-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3ef16-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3ef16-124">Schema name</span></span>  <br/> |<span data-ttu-id="3ef16-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3ef16-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3ef16-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3ef16-126">Validation file</span></span>  <br/> |<span data-ttu-id="3ef16-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3ef16-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3ef16-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3ef16-128">Can be empty</span></span>  <br/> |<span data-ttu-id="3ef16-129">false</span><span class="sxs-lookup"><span data-stu-id="3ef16-129">false</span></span>  <br/> |
   

