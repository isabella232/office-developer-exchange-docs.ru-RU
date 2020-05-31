---
title: арчивеитемреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 68109a92-c49e-4c0e-b6ec-e90d38d4be4d
description: Элемент Арчивеитемреспонсе указывает ответ на запрос ArchiveItem.
ms.openlocfilehash: bfd1b9d76c2b49e00a82bd8f6f57742007d0adf7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761489"
---
# <a name="archiveitemresponse"></a><span data-ttu-id="1f91a-103">арчивеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="1f91a-103">ArchiveItemResponse</span></span>

<span data-ttu-id="1f91a-104">Элемент **арчивеитемреспонсе** указывает ответ на запрос **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="1f91a-104">The **ArchiveItemResponse** element specifies the response to an **ArchiveItem** request.</span></span> 
  
```XML
<ArchiveItemResponse>
    <ResponseMessages></ResponseMessages>
</ArchiveItemResponse>
```

 <span data-ttu-id="1f91a-105">**арчивеитемреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="1f91a-105">**ArchiveItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f91a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1f91a-106">Attributes and elements</span></span>

<span data-ttu-id="1f91a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1f91a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f91a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1f91a-108">Attributes</span></span>

<span data-ttu-id="1f91a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1f91a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f91a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1f91a-110">Child elements</span></span>

|<span data-ttu-id="1f91a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1f91a-111">**Element**</span></span>|<span data-ttu-id="1f91a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1f91a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f91a-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="1f91a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1f91a-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f91a-114">Contains the response messages to an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f91a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1f91a-115">Parent elements</span></span>

<span data-ttu-id="1f91a-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="1f91a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f91a-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="1f91a-117">Remarks</span></span>

<span data-ttu-id="1f91a-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1f91a-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1f91a-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1f91a-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f91a-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1f91a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f91a-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1f91a-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f91a-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1f91a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="1f91a-123">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="1f91a-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="1f91a-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1f91a-124">Validation File</span></span>  <br/> |<span data-ttu-id="1f91a-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1f91a-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f91a-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1f91a-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1f91a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="1f91a-127">See also</span></span>

- [<span data-ttu-id="1f91a-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1f91a-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

