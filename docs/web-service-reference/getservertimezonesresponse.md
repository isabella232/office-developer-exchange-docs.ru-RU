---
title: GetServerTimeZonesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponse
api_type:
- schema
ms.assetid: 97c94d32-10f1-4c3e-ab20-9fd7e8257e50
description: Элемент GetServerTimeZonesResponse определяет ответ на запрос операции GetServerTimeZones.
ms.openlocfilehash: 119809076c82ff75a6dd061fc976f861e13f4e57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833664"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="b05a7-103">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="b05a7-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="b05a7-104">Элемент **GetServerTimeZonesResponse** определяет ответ на запрос [GetServerTimeZones операции](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b05a7-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="b05a7-105">**GetServerTimeZonesResponseType**</span><span class="sxs-lookup"><span data-stu-id="b05a7-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b05a7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b05a7-106">Attributes and elements</span></span>

<span data-ttu-id="b05a7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b05a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b05a7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b05a7-108">Attributes</span></span>

<span data-ttu-id="b05a7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b05a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b05a7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b05a7-110">Child elements</span></span>

|<span data-ttu-id="b05a7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b05a7-111">**Element**</span></span>|<span data-ttu-id="b05a7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b05a7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b05a7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b05a7-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b05a7-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b05a7-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b05a7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b05a7-115">Parent elements</span></span>

<span data-ttu-id="b05a7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="b05a7-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b05a7-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="b05a7-117">Remarks</span></span>

<span data-ttu-id="b05a7-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b05a7-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b05a7-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b05a7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b05a7-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b05a7-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b05a7-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b05a7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="b05a7-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b05a7-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b05a7-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b05a7-123">Validation File</span></span>  <br/> |<span data-ttu-id="b05a7-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b05a7-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b05a7-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b05a7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="b05a7-126">False</span><span class="sxs-lookup"><span data-stu-id="b05a7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b05a7-127">См. также</span><span class="sxs-lookup"><span data-stu-id="b05a7-127">See also</span></span>



- [<span data-ttu-id="b05a7-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b05a7-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

