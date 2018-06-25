---
title: ArchiveItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: Элемент ArchiveItemResponse указывает ответ на запрос ArchiveItem.
ms.openlocfilehash: bfd1b9d76c2b49e00a82bd8f6f57742007d0adf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761489"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="4babf-103">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="4babf-103">ArchiveItemResponse</span></span>

<span data-ttu-id="4babf-104">Элемент **ArchiveItemResponse** указывает ответ на запрос **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="4babf-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="4babf-105">**ArchiveItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="4babf-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4babf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4babf-106">Attributes and elements</span></span>

<span data-ttu-id="4babf-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4babf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4babf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4babf-108">Attributes</span></span>

<span data-ttu-id="4babf-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4babf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4babf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4babf-110">Child elements</span></span>

|<span data-ttu-id="4babf-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4babf-111">**Element**</span></span>|<span data-ttu-id="4babf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4babf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4babf-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4babf-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4babf-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4babf-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4babf-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4babf-115">Parent elements</span></span>

<span data-ttu-id="4babf-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="4babf-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4babf-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="4babf-117">Remarks</span></span>

<span data-ttu-id="4babf-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4babf-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4babf-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4babf-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4babf-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4babf-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4babf-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4babf-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4babf-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4babf-122">Schema Name</span></span>  <br/> |<span data-ttu-id="4babf-123">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="4babf-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="4babf-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4babf-124">Validation File</span></span>  <br/> |<span data-ttu-id="4babf-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4babf-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4babf-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4babf-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4babf-127">См. также</span><span class="sxs-lookup"><span data-stu-id="4babf-127">See also</span></span>

- [<span data-ttu-id="4babf-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4babf-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

