---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: Элемент UserMailbox определяет почтовый ящик пользователя.
ms.openlocfilehash: 9f359a2b0ba315c236d4bf189c3de321417bd390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840425"
---
# <a name="usermailbox"></a><span data-ttu-id="00231-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="00231-103">UserMailbox</span></span>

<span data-ttu-id="00231-104">Элемент **UserMailbox** определяет почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="00231-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="00231-105">**усермаилбокстипе**</span><span class="sxs-lookup"><span data-stu-id="00231-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00231-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="00231-106">Attributes and elements</span></span>

<span data-ttu-id="00231-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="00231-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00231-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="00231-108">Attributes</span></span>

|<span data-ttu-id="00231-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="00231-109">**Attribute**</span></span>|<span data-ttu-id="00231-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00231-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="00231-111">Id</span><span class="sxs-lookup"><span data-stu-id="00231-111">Id</span></span>  <br/> |<span data-ttu-id="00231-112">Текстовое значение атрибута **ID** — идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="00231-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="00231-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="00231-113">IsArchive</span></span>  <br/> |<span data-ttu-id="00231-114">Текстовое значение атрибута **Archive** указывает, является ли почтовый ящик архивным.</span><span class="sxs-lookup"><span data-stu-id="00231-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="00231-115">Текстовое значение **true** для атрибута **Archive** указывает на то, что почтовый ящик является архивным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="00231-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="00231-116">Значение **false** для атрибута **Archive** указывает на то, что почтовый ящик является основным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="00231-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="00231-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="00231-117">Child elements</span></span>

<span data-ttu-id="00231-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="00231-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00231-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="00231-119">Parent elements</span></span>

<span data-ttu-id="00231-120">[Почтовые ящики (аррайофусермаилбоксестипе)](mailboxes-arrayofusermailboxestype.md) | [маилбоксстатистикссеарчресулт](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="00231-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00231-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="00231-121">Remarks</span></span>

<span data-ttu-id="00231-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00231-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="00231-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="00231-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00231-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="00231-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00231-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="00231-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00231-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="00231-126">Schema name</span></span>  <br/> |<span data-ttu-id="00231-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="00231-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="00231-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="00231-128">Validation file</span></span>  <br/> |<span data-ttu-id="00231-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00231-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00231-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="00231-130">Can be empty</span></span>  <br/> |<span data-ttu-id="00231-131">true</span><span class="sxs-lookup"><span data-stu-id="00231-131">true</span></span>  <br/> |
   

