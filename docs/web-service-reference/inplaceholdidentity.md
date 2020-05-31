---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: Элемент InPlaceHoldIdentity указывает идентификатор удержания, который сохраняет элементы почтового ящика.
ms.openlocfilehash: 954e6ad6c3e0b7786d6bbb8230dba913a32359bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833938"
---
# <a name="inplaceholdidentity"></a><span data-ttu-id="ac17a-103">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="ac17a-103">InPlaceHoldIdentity</span></span>

<span data-ttu-id="ac17a-104">Элемент **InPlaceHoldIdentity** указывает идентификатор удержания, который сохраняет элементы почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ac17a-104">The **InPlaceHoldIdentity** element specifies the identity of a hold that preserves the mailbox items.</span></span> 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 <span data-ttu-id="ac17a-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="ac17a-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac17a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ac17a-106">Attributes and elements</span></span>

<span data-ttu-id="ac17a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ac17a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac17a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ac17a-108">Attributes</span></span>

<span data-ttu-id="ac17a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ac17a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac17a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ac17a-110">Child elements</span></span>

<span data-ttu-id="ac17a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ac17a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ac17a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ac17a-112">Parent elements</span></span>

<span data-ttu-id="ac17a-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [дисковерисеарчконфигуратион](discoverysearchconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ac17a-113">[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ac17a-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ac17a-114">Text value</span></span>

<span data-ttu-id="ac17a-115">Текстовое значение элемента **InPlaceHoldIdentity** — идентификатор удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ac17a-115">The text value of the **InPlaceHoldIdentity** element is the mailbox hold identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ac17a-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="ac17a-116">Remarks</span></span>

<span data-ttu-id="ac17a-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ac17a-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ac17a-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ac17a-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac17a-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ac17a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac17a-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ac17a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ac17a-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ac17a-121">Schema name</span></span>  <br/> |<span data-ttu-id="ac17a-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ac17a-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ac17a-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ac17a-123">Validation file</span></span>  <br/> |<span data-ttu-id="ac17a-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ac17a-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ac17a-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ac17a-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ac17a-126">False</span><span class="sxs-lookup"><span data-stu-id="ac17a-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac17a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="ac17a-127">See also</span></span>



[<span data-ttu-id="ac17a-128">Операция SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="ac17a-128">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)


- [<span data-ttu-id="ac17a-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ac17a-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

