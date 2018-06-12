---
title: ExpandDLResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponse
api_type:
- schema
ms.assetid: 1c60dd64-a083-460a-9840-021d30f871d6
description: Элемент ExpandDLResponse определяет ответ на запрос и разверните список рассылки.
ms.openlocfilehash: dbcb0ff8e5c11460c070b8a87da53cecca279b88
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762428"
---
# <a name="expanddlresponse"></a><span data-ttu-id="eb5bb-103">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="eb5bb-103">ExpandDLResponse</span></span>

<span data-ttu-id="eb5bb-104">Элемент **ExpandDLResponse** определяет ответ на запрос и разверните список рассылки.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-104">The **ExpandDLResponse** element defines a response to a request to expand a distribution list.</span></span> 
  
[<span data-ttu-id="eb5bb-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="eb5bb-105">ExpandDLResponse</span></span>](expanddlresponse.md)
  
```xml
<ExpandDLResponse>
   <ResponseMessages/>
</ExpandDLResponse>
```

 <span data-ttu-id="eb5bb-106">**ExpandDLResponseType**</span><span class="sxs-lookup"><span data-stu-id="eb5bb-106">**ExpandDLResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb5bb-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eb5bb-107">Attributes and elements</span></span>

<span data-ttu-id="eb5bb-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb5bb-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eb5bb-109">Attributes</span></span>

<span data-ttu-id="eb5bb-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb5bb-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eb5bb-111">Child elements</span></span>

|<span data-ttu-id="eb5bb-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb5bb-112">**Element**</span></span>|<span data-ttu-id="eb5bb-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb5bb-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb5bb-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eb5bb-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="eb5bb-115">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb5bb-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eb5bb-116">Parent elements</span></span>

<span data-ttu-id="eb5bb-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb5bb-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="eb5bb-118">Remarks</span></span>

<span data-ttu-id="eb5bb-119">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="eb5bb-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb5bb-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eb5bb-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb5bb-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eb5bb-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eb5bb-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eb5bb-122">Schema name</span></span>  <br/> |<span data-ttu-id="eb5bb-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="eb5bb-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="eb5bb-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eb5bb-124">Validation file</span></span>  <br/> |<span data-ttu-id="eb5bb-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eb5bb-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eb5bb-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eb5bb-126">Can be empty</span></span>  <br/> |<span data-ttu-id="eb5bb-127">False</span><span class="sxs-lookup"><span data-stu-id="eb5bb-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb5bb-128">См. также</span><span class="sxs-lookup"><span data-stu-id="eb5bb-128">See also</span></span>



[<span data-ttu-id="eb5bb-129">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="eb5bb-129">ExpandDL</span></span>](expanddl.md)
  
[<span data-ttu-id="eb5bb-130">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="eb5bb-130">ExpandDL operation</span></span>](expanddl-operation.md)

