---
title: GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 769df8eb-9c72-48b5-a49f-82c6b86bc5fc
description: Элемент GetItem определяет запрос на получение элемента из почтового ящика в хранилище Exchange.
ms.openlocfilehash: 39db141bad62c34bec5ae6a937ba94c2d1288090
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762838"
---
# <a name="getitem"></a><span data-ttu-id="f73ea-103">GetItem</span><span class="sxs-lookup"><span data-stu-id="f73ea-103">GetItem</span></span>

<span data-ttu-id="f73ea-104">Элемент **GetItem** определяет запрос на получение элемента из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f73ea-104">The **GetItem** element defines a request to get an item from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetItem>
   <ItemShape/>
   <ItemIds/>
</GetItem>
```

 <span data-ttu-id="f73ea-105">**GetItemType**</span><span class="sxs-lookup"><span data-stu-id="f73ea-105">**GetItemType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f73ea-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f73ea-106">Attributes and elements</span></span>

<span data-ttu-id="f73ea-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f73ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f73ea-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f73ea-108">Attributes</span></span>

<span data-ttu-id="f73ea-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f73ea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f73ea-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f73ea-110">Child elements</span></span>

|<span data-ttu-id="f73ea-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f73ea-111">**Element**</span></span>|<span data-ttu-id="f73ea-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f73ea-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f73ea-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="f73ea-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="f73ea-114">Определяет свойства элемента и содержимого для включения в **GetItem** ответа.</span><span class="sxs-lookup"><span data-stu-id="f73ea-114">Identifies the item properties and content to include in a **GetItem** response.</span></span>  <br/> |
|[<span data-ttu-id="f73ea-115">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="f73ea-115">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="f73ea-116">Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, которые используются для получения элементов из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="f73ea-116">Contains the unique identities of items, occurrence items, and recurring master items that are used to get items from the Exchange store.</span></span> <span data-ttu-id="f73ea-117">Эти элементы представляют контакты, задачи, сообщения, элементы календаря, приглашения на собрания и другие допустимые элементы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f73ea-117">These items represent contacts, tasks, messages, calendar items, meeting requests, and other valid items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f73ea-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f73ea-118">Parent elements</span></span>

<span data-ttu-id="f73ea-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="f73ea-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f73ea-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="f73ea-120">Remarks</span></span>

<span data-ttu-id="f73ea-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f73ea-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f73ea-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f73ea-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f73ea-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f73ea-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f73ea-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f73ea-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f73ea-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="f73ea-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="f73ea-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f73ea-126">Validation File</span></span>  <br/> |<span data-ttu-id="f73ea-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f73ea-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f73ea-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f73ea-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f73ea-129">False</span><span class="sxs-lookup"><span data-stu-id="f73ea-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f73ea-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f73ea-130">See also</span></span>



[<span data-ttu-id="f73ea-131">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="f73ea-131">GetItem operation</span></span>](getitem-operation.md)

