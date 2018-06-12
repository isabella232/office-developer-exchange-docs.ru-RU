---
title: SetTeamMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: Элемент SetTeamMailbox содержит запрос для установки почтового ящика сайта.
ms.openlocfilehash: 708863168f4e89775deee8c5d66427df41515089
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835455"
---
# <a name="setteammailbox"></a><span data-ttu-id="cfea8-103">SetTeamMailbox</span><span class="sxs-lookup"><span data-stu-id="cfea8-103">SetTeamMailbox</span></span>

<span data-ttu-id="cfea8-104">Элемент **SetTeamMailbox** содержит запрос для установки почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="cfea8-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="cfea8-105">**SetTeamMailboxRequestType**</span><span class="sxs-lookup"><span data-stu-id="cfea8-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cfea8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cfea8-106">Attributes and elements</span></span>

<span data-ttu-id="cfea8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cfea8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cfea8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cfea8-108">Attributes</span></span>

<span data-ttu-id="cfea8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cfea8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cfea8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cfea8-110">Child elements</span></span>

<span data-ttu-id="cfea8-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [состояния (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="cfea8-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cfea8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cfea8-112">Parent elements</span></span>

<span data-ttu-id="cfea8-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="cfea8-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cfea8-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="cfea8-114">Remarks</span></span>

<span data-ttu-id="cfea8-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cfea8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cfea8-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cfea8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cfea8-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cfea8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cfea8-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cfea8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cfea8-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cfea8-119">Schema name</span></span>  <br/> |<span data-ttu-id="cfea8-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cfea8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cfea8-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cfea8-121">Validation file</span></span>  <br/> |<span data-ttu-id="cfea8-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cfea8-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cfea8-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cfea8-123">Can be empty</span></span>  <br/> ||
   

