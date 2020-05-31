---
title: жетсеарчаблемаилбоксесреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0fcc2f53-742b-46ae-bbab-c3295a3d69e7
description: Элемент Жетсеарчаблемаилбоксесреспонсе содержит ответ на запрос GetSearchableMailboxes.
ms.openlocfilehash: 35a671cd534d1b48b29ef836c24d97d7cbd52401
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762914"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="34353-103">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="34353-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="34353-104">Элемент **жетсеарчаблемаилбоксесреспонсе** содержит ответ на запрос **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="34353-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<GetSearchableMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SearchableMailboxes/>
   <FailedMailboxes/>
</GetSearchableMailboxesResponse>
```

 <span data-ttu-id="34353-105">**жетсеарчаблемаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="34353-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34353-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="34353-106">Attributes and elements</span></span>

<span data-ttu-id="34353-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="34353-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34353-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="34353-108">Attributes</span></span>

<span data-ttu-id="34353-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="34353-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34353-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="34353-110">Child elements</span></span>

<span data-ttu-id="34353-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md) | [FailedMailboxes](failedmailboxes.md) дескриптивелинккэй мессажексмл | [сеарчаблемаилбоксес](searchablemailboxes.md)фаиледмаилбоксес | </span><span class="sxs-lookup"><span data-stu-id="34353-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34353-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="34353-112">Parent elements</span></span>

<span data-ttu-id="34353-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="34353-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34353-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="34353-114">Remarks</span></span>

<span data-ttu-id="34353-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34353-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34353-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="34353-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34353-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="34353-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34353-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="34353-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34353-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="34353-119">Schema name</span></span>  <br/> |<span data-ttu-id="34353-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="34353-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34353-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="34353-121">Validation file</span></span>  <br/> |<span data-ttu-id="34353-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34353-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34353-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="34353-123">Can be empty</span></span>  <br/> |<span data-ttu-id="34353-124">false</span><span class="sxs-lookup"><span data-stu-id="34353-124">false</span></span>  <br/> |
   

