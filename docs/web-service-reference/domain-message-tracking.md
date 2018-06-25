---
title: Домен (отслеживания сообщений)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 4e8e9efa-8885-4ca5-bf90-424e63768dc3
description: Элемент домена представляет домен для поиска.
ms.openlocfilehash: dc161557b59acc580d918f2e196457714bce4ba9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762200"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="c41f3-103">Домен (отслеживания сообщений)</span><span class="sxs-lookup"><span data-stu-id="c41f3-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="c41f3-104">Элемент **домена** представляет домен для поиска.</span><span class="sxs-lookup"><span data-stu-id="c41f3-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="c41f3-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="c41f3-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c41f3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c41f3-106">Attributes and elements</span></span>

<span data-ttu-id="c41f3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c41f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c41f3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c41f3-108">Attributes</span></span>

<span data-ttu-id="c41f3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c41f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c41f3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c41f3-110">Child elements</span></span>

<span data-ttu-id="c41f3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c41f3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c41f3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c41f3-112">Parent elements</span></span>

|<span data-ttu-id="c41f3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c41f3-113">**Element**</span></span>|<span data-ttu-id="c41f3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c41f3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c41f3-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c41f3-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="c41f3-116">Содержит критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="c41f3-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c41f3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c41f3-117">Text value</span></span>

<span data-ttu-id="c41f3-118">Текстовое значение, представляющее строку является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="c41f3-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c41f3-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="c41f3-119">Remarks</span></span>

<span data-ttu-id="c41f3-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c41f3-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c41f3-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c41f3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c41f3-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c41f3-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c41f3-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c41f3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c41f3-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c41f3-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c41f3-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c41f3-125">Validation File</span></span>  <br/> |<span data-ttu-id="c41f3-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c41f3-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c41f3-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c41f3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c41f3-128">False</span><span class="sxs-lookup"><span data-stu-id="c41f3-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c41f3-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c41f3-129">See also</span></span>

- [<span data-ttu-id="c41f3-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c41f3-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

