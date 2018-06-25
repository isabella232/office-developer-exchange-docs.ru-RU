---
title: GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 82a737c7-da41-4777-8ad8-89851a0b602b
description: Элемент GetRooms является корневым элементом в запросе для получения списка комнат в пределах определенного почтового ящика помещения.
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762909"
---
# <a name="getrooms"></a><span data-ttu-id="04fd7-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="04fd7-103">GetRooms</span></span>

<span data-ttu-id="04fd7-104">Элемент **GetRooms** является корневым элементом в запросе для получения списка комнат в пределах определенного почтового ящика помещения.</span><span class="sxs-lookup"><span data-stu-id="04fd7-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="04fd7-105">**GetRoomsType**</span><span class="sxs-lookup"><span data-stu-id="04fd7-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04fd7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="04fd7-106">Attributes and elements</span></span>

<span data-ttu-id="04fd7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="04fd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04fd7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="04fd7-108">Attributes</span></span>

<span data-ttu-id="04fd7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="04fd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04fd7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="04fd7-110">Child elements</span></span>

|<span data-ttu-id="04fd7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="04fd7-111">**Element**</span></span>|<span data-ttu-id="04fd7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04fd7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04fd7-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="04fd7-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="04fd7-114">Представляет адрес электронной почты, который определяет список конференц-залы</span><span class="sxs-lookup"><span data-stu-id="04fd7-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="04fd7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="04fd7-115">Parent elements</span></span>

<span data-ttu-id="04fd7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="04fd7-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="04fd7-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="04fd7-117">Text value</span></span>

<span data-ttu-id="04fd7-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="04fd7-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04fd7-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="04fd7-119">Remarks</span></span>

<span data-ttu-id="04fd7-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="04fd7-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04fd7-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="04fd7-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04fd7-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="04fd7-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="04fd7-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="04fd7-123">Schema Name</span></span>  <br/> |<span data-ttu-id="04fd7-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="04fd7-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="04fd7-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="04fd7-125">Validation File</span></span>  <br/> |<span data-ttu-id="04fd7-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="04fd7-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="04fd7-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="04fd7-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="04fd7-128">False</span><span class="sxs-lookup"><span data-stu-id="04fd7-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04fd7-129">См. также</span><span class="sxs-lookup"><span data-stu-id="04fd7-129">See also</span></span>



- [<span data-ttu-id="04fd7-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="04fd7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

