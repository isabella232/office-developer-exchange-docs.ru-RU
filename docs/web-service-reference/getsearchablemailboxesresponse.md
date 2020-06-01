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
ms.openlocfilehash: 680fde9d9ad34dd0384e00da023796d004b66b1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458266"
---
# <a name="getsearchablemailboxesresponse"></a><span data-ttu-id="e89af-103">жетсеарчаблемаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="e89af-103">GetSearchableMailboxesResponse</span></span>

<span data-ttu-id="e89af-104">Элемент **жетсеарчаблемаилбоксесреспонсе** содержит ответ на запрос **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="e89af-104">The **GetSearchableMailboxesResponse** element contains the response to a **GetSearchableMailboxes** request.</span></span> 
  
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

 <span data-ttu-id="e89af-105">**жетсеарчаблемаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="e89af-105">**GetSearchableMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e89af-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e89af-106">Attributes and elements</span></span>

<span data-ttu-id="e89af-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e89af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e89af-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e89af-108">Attributes</span></span>

<span data-ttu-id="e89af-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e89af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e89af-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e89af-110">Child elements</span></span>

<span data-ttu-id="e89af-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Сеарчаблемаилбоксес](searchablemailboxes.md)  |  [Фаиледмаилбоксес](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="e89af-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [SearchableMailboxes](searchablemailboxes.md) | [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e89af-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e89af-112">Parent elements</span></span>

<span data-ttu-id="e89af-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="e89af-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e89af-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="e89af-114">Remarks</span></span>

<span data-ttu-id="e89af-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e89af-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e89af-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e89af-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e89af-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e89af-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e89af-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e89af-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e89af-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e89af-119">Schema name</span></span>  <br/> |<span data-ttu-id="e89af-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e89af-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e89af-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e89af-121">Validation file</span></span>  <br/> |<span data-ttu-id="e89af-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e89af-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e89af-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e89af-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e89af-124">false</span><span class="sxs-lookup"><span data-stu-id="e89af-124">false</span></span>  <br/> |
   

