---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: Элемент NonIndexableItemDetailsResult указывает результаты операции GetNonIndexableItemDetails WSDL.
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834535"
---
# <a name="nonindexableitemdetailsresult"></a><span data-ttu-id="1bfe8-103">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="1bfe8-103">NonIndexableItemDetailsResult</span></span>

<span data-ttu-id="1bfe8-104">Элемент **NonIndexableItemDetailsResult** указывает результаты операции WSDL **GetNonIndexableItemDetails** .</span><span class="sxs-lookup"><span data-stu-id="1bfe8-104">The **NonIndexableItemDetailsResult** element specifies the results of the **GetNonIndexableItemDetails** WSDL operation.</span></span> 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 <span data-ttu-id="1bfe8-105">**NonIndexableItemDetailResultType**</span><span class="sxs-lookup"><span data-stu-id="1bfe8-105">**NonIndexableItemDetailResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1bfe8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1bfe8-106">Attributes and elements</span></span>

<span data-ttu-id="1bfe8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1bfe8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1bfe8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1bfe8-108">Attributes</span></span>

<span data-ttu-id="1bfe8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1bfe8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1bfe8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1bfe8-110">Child elements</span></span>

<span data-ttu-id="1bfe8-111">[Элементы (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="1bfe8-111">[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1bfe8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1bfe8-112">Parent elements</span></span>

<span data-ttu-id="1bfe8-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="1bfe8-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1bfe8-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="1bfe8-114">Remarks</span></span>

<span data-ttu-id="1bfe8-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1bfe8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1bfe8-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1bfe8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1bfe8-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1bfe8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1bfe8-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1bfe8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1bfe8-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1bfe8-119">Schema name</span></span>  <br/> |<span data-ttu-id="1bfe8-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1bfe8-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1bfe8-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1bfe8-121">Validation file</span></span>  <br/> |<span data-ttu-id="1bfe8-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1bfe8-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1bfe8-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1bfe8-123">Can be empty</span></span>  <br/> |<span data-ttu-id="1bfe8-124">False</span><span class="sxs-lookup"><span data-stu-id="1bfe8-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1bfe8-125">См. также</span><span class="sxs-lookup"><span data-stu-id="1bfe8-125">See also</span></span>



[<span data-ttu-id="1bfe8-126">Операция GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="1bfe8-126">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)


- [<span data-ttu-id="1bfe8-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1bfe8-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

