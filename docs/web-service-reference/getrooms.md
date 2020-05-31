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
description: Элемент "множество помещений" является корневым элементом запроса для получения списка комнат в определенном списке помещений.
ms.openlocfilehash: a787097752cfeee9489e5f118549c2d939ba4c9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762909"
---
# <a name="getrooms"></a><span data-ttu-id="f65d9-103">GetRooms</span><span class="sxs-lookup"><span data-stu-id="f65d9-103">GetRooms</span></span>

<span data-ttu-id="f65d9-104">Элемент "множество **помещений** " является корневым элементом запроса для получения списка комнат в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="f65d9-104">The **GetRooms** element is the root element in a request to get a list of rooms within a particular room list.</span></span> 
  
```XML
<GetRooms>
   <RoomList/>
</GetRooms>
```

 <span data-ttu-id="f65d9-105">**жетрумстипе**</span><span class="sxs-lookup"><span data-stu-id="f65d9-105">**GetRoomsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f65d9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f65d9-106">Attributes and elements</span></span>

<span data-ttu-id="f65d9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f65d9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f65d9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f65d9-108">Attributes</span></span>

<span data-ttu-id="f65d9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f65d9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f65d9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f65d9-110">Child elements</span></span>

|<span data-ttu-id="f65d9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f65d9-111">**Element**</span></span>|<span data-ttu-id="f65d9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f65d9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f65d9-113">RoomList</span><span class="sxs-lookup"><span data-stu-id="f65d9-113">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="f65d9-114">Представляет адрес электронной почты, определяющий список комнат для собраний</span><span class="sxs-lookup"><span data-stu-id="f65d9-114">Represents an e-mail address that identifies a list of meeting rooms</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f65d9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f65d9-115">Parent elements</span></span>

<span data-ttu-id="f65d9-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="f65d9-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f65d9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f65d9-117">Text value</span></span>

<span data-ttu-id="f65d9-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="f65d9-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f65d9-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f65d9-119">Remarks</span></span>

<span data-ttu-id="f65d9-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f65d9-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f65d9-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f65d9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f65d9-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f65d9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f65d9-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f65d9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f65d9-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f65d9-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f65d9-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f65d9-125">Validation File</span></span>  <br/> |<span data-ttu-id="f65d9-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f65d9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f65d9-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f65d9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f65d9-128">False</span><span class="sxs-lookup"><span data-stu-id="f65d9-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f65d9-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f65d9-129">See also</span></span>



- [<span data-ttu-id="f65d9-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f65d9-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

