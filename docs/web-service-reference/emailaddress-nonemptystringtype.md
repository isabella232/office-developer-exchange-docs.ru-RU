---
title: EmailAddress (NonEmptyStringType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EmailAddress
api_type:
- schema
ms.assetid: c0c708d1-b016-4902-a294-9af44aea2050
description: Элемент EmailAddress определяет основной SMTP-адрес пользователя почтового ящика.
ms.openlocfilehash: fcf2839c1e2e40a22d6b6a856608f52f2c9c2a1a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762281"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="e4f5e-103">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="e4f5e-104">Элемент **EmailAddress** определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="e4f5e-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="e4f5e-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4f5e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4f5e-106">Attributes and elements</span></span>

<span data-ttu-id="e4f5e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4f5e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4f5e-108">Attributes</span></span>

<span data-ttu-id="e4f5e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4f5e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4f5e-110">Child elements</span></span>

<span data-ttu-id="e4f5e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4f5e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4f5e-112">Parent elements</span></span>

|<span data-ttu-id="e4f5e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4f5e-113">**Element**</span></span>|<span data-ttu-id="e4f5e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4f5e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4f5e-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="e4f5e-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="e4f5e-116">Определяет, как отправляющего вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="e4f5e-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="e4f5e-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="e4f5e-118">Определяет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="e4f5e-119">Ниже приведены некоторые выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="e4f5e-120">Ниже приведены дополнительные родительские элементы элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="e4f5e-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="e4f5e-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="e4f5e-123">- [Отправитель](sender.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="e4f5e-124">- [От](from.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-124">- [From](from.md)</span></span> <br/><span data-ttu-id="e4f5e-125">- [Организатор](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="e4f5e-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="e4f5e-127">- [Решение](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="e4f5e-128">- [DLExpansion](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="e4f5e-129">- [Участник](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="e4f5e-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="e4f5e-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="e4f5e-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="e4f5e-131">Определяет список конференц-залы, адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4f5e-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4f5e-132">Text value</span></span>

<span data-ttu-id="e4f5e-133">Текстовое значение, представляющее SMTP-адрес является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4f5e-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="e4f5e-134">Remarks</span></span>

<span data-ttu-id="e4f5e-135">Элемент **EmailAddress** может представлять SMTP или прежних версий Exchange различающееся имя (DN) адресов.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="e4f5e-136">Элемент **EmailAddress** является единственным обязательным элементом [почтового ящика](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="e4f5e-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="e4f5e-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4f5e-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4f5e-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4f5e-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4f5e-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4f5e-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4f5e-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4f5e-140">Schema Name</span></span>  <br/> |<span data-ttu-id="e4f5e-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4f5e-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4f5e-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4f5e-142">Validation File</span></span>  <br/> |<span data-ttu-id="e4f5e-143">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4f5e-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4f5e-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4f5e-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4f5e-145">False</span><span class="sxs-lookup"><span data-stu-id="e4f5e-145">False</span></span>  <br/> |
   

