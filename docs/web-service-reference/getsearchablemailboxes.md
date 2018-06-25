---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: Элемент GetSearchableMailboxes содержит запрос на получение списка почтовых ящиков, что клиент имеет разрешение на выполнение поиска методом электронного обнаружения.
ms.openlocfilehash: 8cce18bb62d3840cb9883d20a380cc4f2193303e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762906"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="877d6-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="877d6-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="877d6-104">Элемент **GetSearchableMailboxes** содержит запрос на получение списка почтовых ящиков, что клиент имеет разрешение на выполнение поиска методом электронного обнаружения.</span><span class="sxs-lookup"><span data-stu-id="877d6-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="877d6-105">**GetSearchableMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="877d6-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="877d6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="877d6-106">Attributes and elements</span></span>

<span data-ttu-id="877d6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="877d6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="877d6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="877d6-108">Attributes</span></span>

<span data-ttu-id="877d6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="877d6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="877d6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="877d6-110">Child elements</span></span>

<span data-ttu-id="877d6-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="877d6-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="877d6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="877d6-112">Parent elements</span></span>

<span data-ttu-id="877d6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="877d6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="877d6-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="877d6-114">Remarks</span></span>

<span data-ttu-id="877d6-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="877d6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="877d6-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="877d6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="877d6-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="877d6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="877d6-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="877d6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="877d6-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="877d6-119">Schema name</span></span>  <br/> |<span data-ttu-id="877d6-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="877d6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="877d6-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="877d6-121">Validation file</span></span>  <br/> |<span data-ttu-id="877d6-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="877d6-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="877d6-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="877d6-123">Can be empty</span></span>  <br/> ||
   

