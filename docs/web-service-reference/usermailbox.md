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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840425"
---
# <a name="usermailbox"></a><span data-ttu-id="4f6cf-103">UserMailbox</span><span class="sxs-lookup"><span data-stu-id="4f6cf-103">UserMailbox</span></span>

<span data-ttu-id="4f6cf-104">Элемент **UserMailbox** определяет почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-104">The **UserMailbox** element identifies a user mailbox.</span></span> 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 <span data-ttu-id="4f6cf-105">**UserMailboxType**</span><span class="sxs-lookup"><span data-stu-id="4f6cf-105">**UserMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f6cf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f6cf-106">Attributes and elements</span></span>

<span data-ttu-id="4f6cf-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f6cf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f6cf-108">Attributes</span></span>

|<span data-ttu-id="4f6cf-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="4f6cf-109">**Attribute**</span></span>|<span data-ttu-id="4f6cf-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f6cf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4f6cf-111">Id</span><span class="sxs-lookup"><span data-stu-id="4f6cf-111">Id</span></span>  <br/> |<span data-ttu-id="4f6cf-112">Текстовое значение атрибута **Id** — идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-112">The text value of the **Id** attribute is the identifier of the mailbox.</span></span>  <br/> |
|<span data-ttu-id="4f6cf-113">IsArchive</span><span class="sxs-lookup"><span data-stu-id="4f6cf-113">IsArchive</span></span>  <br/> |<span data-ttu-id="4f6cf-114">Текстовое значение атрибута **IsArchive** указывает, является ли почтовом ящике архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-114">The text value of the **IsArchive** attribute indicates whether the mailbox is an archive mailbox.</span></span> <span data-ttu-id="4f6cf-115">Текстовое значение **true** для атрибута **IsArchive** указывает, что почтовый ящик архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-115">A text value of **true** for the **IsArchive** attribute indicates that the mailbox is an archive mailbox.</span></span> <span data-ttu-id="4f6cf-116">Значение **false** для атрибута **IsArchive** указывает, что почтовый ящик является основной почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-116">A value of **false** for the **IsArchive** attribute indicates that the mailbox is a primary mailbox.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4f6cf-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f6cf-117">Child elements</span></span>

<span data-ttu-id="4f6cf-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4f6cf-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f6cf-119">Parent elements</span></span>

<span data-ttu-id="4f6cf-120">[Почтовые ящики (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span><span class="sxs-lookup"><span data-stu-id="4f6cf-120">[Mailboxes (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4f6cf-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="4f6cf-121">Remarks</span></span>

<span data-ttu-id="4f6cf-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4f6cf-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f6cf-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f6cf-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f6cf-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f6cf-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f6cf-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4f6cf-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f6cf-126">Schema name</span></span>  <br/> |<span data-ttu-id="4f6cf-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4f6cf-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4f6cf-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f6cf-128">Validation file</span></span>  <br/> |<span data-ttu-id="4f6cf-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4f6cf-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4f6cf-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f6cf-130">Can be empty</span></span>  <br/> |<span data-ttu-id="4f6cf-131">true</span><span class="sxs-lookup"><span data-stu-id="4f6cf-131">true</span></span>  <br/> |
   

