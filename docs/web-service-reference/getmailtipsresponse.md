---
title: GetMailTipsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: Элемент GetMailTipsResponse представляет ответное сообщение для операции GetMailTips.
ms.openlocfilehash: e7a18e8818761af931d32b26aeaf58a2853fa684
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762845"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="5fb6e-103">GetMailTipsResponse</span><span class="sxs-lookup"><span data-stu-id="5fb6e-103">GetMailTipsResponse</span></span>

<span data-ttu-id="5fb6e-104">Элемент **GetMailTipsResponse** представляет ответное сообщение для [операции GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5fb6e-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="5fb6e-105">**GetMailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5fb6e-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5fb6e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5fb6e-106">Attributes and elements</span></span>

<span data-ttu-id="5fb6e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5fb6e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5fb6e-108">Attributes</span></span>

<span data-ttu-id="5fb6e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5fb6e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5fb6e-110">Child elements</span></span>

|<span data-ttu-id="5fb6e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5fb6e-111">**Element**</span></span>|<span data-ttu-id="5fb6e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5fb6e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5fb6e-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="5fb6e-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="5fb6e-114">Представляет список ответа советы почтовых сообщений.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5fb6e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5fb6e-115">Parent elements</span></span>

<span data-ttu-id="5fb6e-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5fb6e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5fb6e-117">Text value</span></span>

<span data-ttu-id="5fb6e-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5fb6e-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="5fb6e-119">Remarks</span></span>

<span data-ttu-id="5fb6e-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5fb6e-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5fb6e-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5fb6e-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5fb6e-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5fb6e-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5fb6e-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5fb6e-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5fb6e-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5fb6e-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5fb6e-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5fb6e-125">Validation File</span></span>  <br/> |<span data-ttu-id="5fb6e-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5fb6e-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5fb6e-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5fb6e-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5fb6e-128">False</span><span class="sxs-lookup"><span data-stu-id="5fb6e-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5fb6e-129">См. также</span><span class="sxs-lookup"><span data-stu-id="5fb6e-129">See also</span></span>



[<span data-ttu-id="5fb6e-130">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="5fb6e-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="5fb6e-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5fb6e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

