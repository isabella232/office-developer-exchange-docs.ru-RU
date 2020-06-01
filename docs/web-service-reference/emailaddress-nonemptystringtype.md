---
title: EmailAddress (Нонемптистрингтипе)
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
ms.openlocfilehash: fcc3e650d5fc32344022ed6f015d4096a4461f63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463134"
---
# <a name="emailaddress-nonemptystringtype"></a><span data-ttu-id="5aaa6-103">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-103">EmailAddress (NonEmptyStringType)</span></span>

<span data-ttu-id="5aaa6-104">Элемент **EmailAddress** определяет основной SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-104">The **EmailAddress** element defines the primary SMTP address of a mailbox user.</span></span> 
  
```XML
<EmailAddress/>
```

 <span data-ttu-id="5aaa6-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="5aaa6-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5aaa6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5aaa6-106">Attributes and elements</span></span>

<span data-ttu-id="5aaa6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5aaa6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5aaa6-108">Attributes</span></span>

<span data-ttu-id="5aaa6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5aaa6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5aaa6-110">Child elements</span></span>

<span data-ttu-id="5aaa6-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5aaa6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5aaa6-112">Parent elements</span></span>

|<span data-ttu-id="5aaa6-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5aaa6-113">**Element**</span></span>|<span data-ttu-id="5aaa6-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5aaa6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5aaa6-115">актингас</span><span class="sxs-lookup"><span data-stu-id="5aaa6-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="5aaa6-116">Указывает, кому отправляется вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="5aaa6-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="5aaa6-117">Mailbox</span></span>](mailbox.md) <br/> | <span data-ttu-id="5aaa6-118">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-118">Identifies a fully resolved e-mail address.</span></span>  <br/><br/><span data-ttu-id="5aaa6-119">Ниже приведено несколько выражений XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="5aaa6-119">The following are some XPath expressions to this element:</span></span><br/><br/>`/CreateItem/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`/CreateFolder/ParentFolderId/DistinguishedFolderId/Mailbox`<br/><br/>`CreateItem/Items/AcceptItem/ToRecipients/Mailbox`<br/><br/>`SyncFolderItemsResponseMessage/Changes/Create/CalendarItem/ConflictingMeetings/AcceptItem/CcRecipients/Mailbox`<br/><br/><span data-ttu-id="5aaa6-120">Ниже приведены дополнительные родительские элементы элемента Mailbox:</span><span class="sxs-lookup"><span data-stu-id="5aaa6-120">The following are additional parent elements of the Mailbox element:</span></span><br/><br/><span data-ttu-id="5aaa6-121">- [BccRecipients](bccrecipients.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-121">- [BccRecipients](bccrecipients.md)</span></span> <br/><span data-ttu-id="5aaa6-122">- [ReplyTo](replyto.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-122">- [ReplyTo](replyto.md)</span></span> <br/><span data-ttu-id="5aaa6-123">- [Организатор](sender.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-123">- [Sender](sender.md)</span></span> <br/><span data-ttu-id="5aaa6-124">- [От](from.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-124">- [From](from.md)</span></span> <br/><span data-ttu-id="5aaa6-125">- [Коллекции](organizer.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-125">- [Organizer](organizer.md)</span></span> <br/><span data-ttu-id="5aaa6-126">- [дистингуишедфолдерид](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-126">- [DistinguishedFolderId](distinguishedfolderid.md)</span></span> <br/><span data-ttu-id="5aaa6-127">- [Решение](resolution.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-127">- [Resolution](resolution.md)</span></span> <br/><span data-ttu-id="5aaa6-128">- [длекспансион](dlexpansion.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-128">- [DLExpansion](dlexpansion.md)</span></span> <br/><span data-ttu-id="5aaa6-129">- [Участника](attendee.md)</span><span class="sxs-lookup"><span data-stu-id="5aaa6-129">- [Attendee](attendee.md)</span></span> <br/> |
|[<span data-ttu-id="5aaa6-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="5aaa6-130">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="5aaa6-131">Определяет список комнат для собраний по адресу электронной почты.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-131">Identifies a list of meeting rooms by email address.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5aaa6-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5aaa6-132">Text value</span></span>

<span data-ttu-id="5aaa6-133">Необходимо указать текстовое значение, представляющее SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-133">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5aaa6-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="5aaa6-134">Remarks</span></span>

<span data-ttu-id="5aaa6-135">Элемент **EmailAddress** может представлять SMTP-адреса или адреса прежнего различающегося имени Exchange (также известные как DN).</span><span class="sxs-lookup"><span data-stu-id="5aaa6-135">The **EmailAddress** element can represent SMTP or legacy Exchange distinguished name (also known as DN) addresses.</span></span> <span data-ttu-id="5aaa6-136">Элементом **EmailAddress** является единственный обязательный элемент [почтового ящика](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="5aaa6-136">The **EmailAddress** element is the only required [Mailbox](mailbox.md) element.</span></span> 
  
<span data-ttu-id="5aaa6-137">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5aaa6-137">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5aaa6-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5aaa6-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5aaa6-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5aaa6-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5aaa6-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5aaa6-140">Schema Name</span></span>  <br/> |<span data-ttu-id="5aaa6-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5aaa6-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="5aaa6-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5aaa6-142">Validation File</span></span>  <br/> |<span data-ttu-id="5aaa6-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5aaa6-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5aaa6-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5aaa6-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="5aaa6-145">False</span><span class="sxs-lookup"><span data-stu-id="5aaa6-145">False</span></span>  <br/> |
   

