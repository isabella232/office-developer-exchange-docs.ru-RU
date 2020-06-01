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
ms.openlocfilehash: 37ad5c6e8f880831a98ff2e649a92cee99930889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44438084"
---
# <a name="setholdonmailboxesresponse"></a><span data-ttu-id="34d73-103">сесолдонмаилбоксесреспонсе</span><span class="sxs-lookup"><span data-stu-id="34d73-103">SetHoldOnMailboxesResponse</span></span>

<span data-ttu-id="34d73-104">Элемент **сесолдонмаилбоксесреспонсе** представляет ответ на запрос **SetHoldOnMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="34d73-104">The **SetHoldOnMailboxesResponse** element represents a response to a **SetHoldOnMailboxes** request.</span></span> 
  
```XML
<SetHoldOnMailboxesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailboxHoldResult/>
</SetHoldOnMailboxesResponse>
```

 <span data-ttu-id="34d73-105">**сесолдонмаилбоксесреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="34d73-105">**SetHoldOnMailboxesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34d73-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="34d73-106">Attributes and elements</span></span>

<span data-ttu-id="34d73-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="34d73-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34d73-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="34d73-108">Attributes</span></span>

<span data-ttu-id="34d73-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="34d73-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34d73-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="34d73-110">Child elements</span></span>

<span data-ttu-id="34d73-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Маилбоксхолдресулт](mailboxholdresult.md)</span><span class="sxs-lookup"><span data-stu-id="34d73-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [MailboxHoldResult](mailboxholdresult.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="34d73-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="34d73-112">Parent elements</span></span>

<span data-ttu-id="34d73-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="34d73-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="34d73-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="34d73-114">Remarks</span></span>

<span data-ttu-id="34d73-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="34d73-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="34d73-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="34d73-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34d73-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="34d73-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34d73-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="34d73-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34d73-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="34d73-119">Schema name</span></span>  <br/> |<span data-ttu-id="34d73-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="34d73-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34d73-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="34d73-121">Validation file</span></span>  <br/> |<span data-ttu-id="34d73-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34d73-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34d73-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="34d73-123">Can be empty</span></span>  <br/> |<span data-ttu-id="34d73-124">false</span><span class="sxs-lookup"><span data-stu-id="34d73-124">false</span></span>  <br/> |
   

