---
title: сесолдонмаилбоксесреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 909194d6-e2b1-4774-bf29-04ed4318df1d
description: Элемент Сесолдонмаилбоксесреспонсе представляет ответ на запрос SetHoldOnMailboxes.
ms.openlocfilehash: bb1d64b98f5e1ab4cdbe4a297ded46d00b27b364
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835418"
---
# <a name="setholdonmailboxesresponse"></a><span data-ttu-id="1ee10-103">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="1ee10-103">SetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="1ee10-104">Элемент **сесолдонмаилбоксесреспонсе** представляет ответ на запрос **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="1ee10-104">The **SetHoldOnMailboxesResponse** element represents a response to a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponse>
```

 <span data-ttu-id="1ee10-105">**сесолдонмаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="1ee10-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ee10-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1ee10-106">Attributes and elements</span></span>

<span data-ttu-id="1ee10-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1ee10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ee10-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ee10-108">Attributes</span></span>

<span data-ttu-id="1ee10-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ee10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ee10-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1ee10-110">Child elements</span></span>

<span data-ttu-id="1ee10-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [MailboxHoldResult](mailboxholdresult.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл маилбоксхолдресулт |  | </span><span class="sxs-lookup"><span data-stu-id="1ee10-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ee10-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1ee10-112">Parent elements</span></span>

<span data-ttu-id="1ee10-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ee10-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1ee10-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="1ee10-114">Remarks</span></span>

<span data-ttu-id="1ee10-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1ee10-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1ee10-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ee10-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ee10-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1ee10-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ee10-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1ee10-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ee10-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1ee10-119">Schema name</span></span>  <br/> |<span data-ttu-id="1ee10-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1ee10-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ee10-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1ee10-121">Validation file</span></span>  <br/> |<span data-ttu-id="1ee10-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1ee10-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ee10-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1ee10-123">Can be empty</span></span>  <br/> |<span data-ttu-id="1ee10-124">false</span><span class="sxs-lookup"><span data-stu-id="1ee10-124">false</span></span>  <br/> |
   

