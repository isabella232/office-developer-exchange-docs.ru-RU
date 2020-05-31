---
title: сеттеаммаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5d6ee7cc-8f88-4de2-ae5c-cabf2f2193d0
description: Элемент Сеттеаммаилбокс содержит запрос на задание почтового ящика сайта.
ms.openlocfilehash: 708863168f4e89775deee8c5d66427df41515089
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835455"
---
# <a name="setteammailbox"></a><span data-ttu-id="98ae4-103">сеттеаммаилбокс</span><span class="sxs-lookup"><span data-stu-id="98ae4-103">SetTeamMailbox</span></span>

<span data-ttu-id="98ae4-104">Элемент **сеттеаммаилбокс** содержит запрос на задание почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="98ae4-104">The **SetTeamMailbox** element contains a request to set a site mailbox.</span></span> 
  
```XML
<SetTeamMailbox>
   <EmailAddress/>
   <SharePointSiteUrl/>
   <State/>
</SetTeamMailbox>
```

 <span data-ttu-id="98ae4-105">**сеттеаммаилбоксрекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="98ae4-105">**SetTeamMailboxRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98ae4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98ae4-106">Attributes and elements</span></span>

<span data-ttu-id="98ae4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="98ae4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98ae4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98ae4-108">Attributes</span></span>

<span data-ttu-id="98ae4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="98ae4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98ae4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98ae4-110">Child elements</span></span>

<span data-ttu-id="98ae4-111">[EmailAddressType](emailaddress-emailaddresstype.md) | состояние[шарепоинтситеурл](sharepointsiteurl.md) | [(теаммаилбокслифециклестатетипе)](state-teammailboxlifecyclestatetype.md)</span><span class="sxs-lookup"><span data-stu-id="98ae4-111">[EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md) | [SharePointSiteUrl](sharepointsiteurl.md) | [State (TeamMailboxLifecycleStateType)](state-teammailboxlifecyclestatetype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98ae4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98ae4-112">Parent elements</span></span>

<span data-ttu-id="98ae4-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="98ae4-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98ae4-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="98ae4-114">Remarks</span></span>

<span data-ttu-id="98ae4-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="98ae4-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="98ae4-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="98ae4-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="98ae4-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98ae4-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98ae4-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98ae4-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98ae4-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98ae4-119">Schema name</span></span>  <br/> |<span data-ttu-id="98ae4-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="98ae4-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="98ae4-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98ae4-121">Validation file</span></span>  <br/> |<span data-ttu-id="98ae4-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="98ae4-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98ae4-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98ae4-123">Can be empty</span></span>  <br/> ||
   

