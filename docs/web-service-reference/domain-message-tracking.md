---
title: Domain (отслеживание сообщений)
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
description: Элемент domain представляет домен, который требуется найти.
ms.openlocfilehash: dc161557b59acc580d918f2e196457714bce4ba9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762200"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="fc563-103">Domain (отслеживание сообщений)</span><span class="sxs-lookup"><span data-stu-id="fc563-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="fc563-104">Элемент **domain** представляет домен, который требуется найти.</span><span class="sxs-lookup"><span data-stu-id="fc563-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="fc563-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="fc563-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc563-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc563-106">Attributes and elements</span></span>

<span data-ttu-id="fc563-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fc563-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc563-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc563-108">Attributes</span></span>

<span data-ttu-id="fc563-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc563-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc563-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc563-110">Child elements</span></span>

<span data-ttu-id="fc563-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc563-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc563-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc563-112">Parent elements</span></span>

|<span data-ttu-id="fc563-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc563-113">**Element**</span></span>|<span data-ttu-id="fc563-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc563-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc563-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="fc563-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="fc563-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="fc563-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc563-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc563-117">Text value</span></span>

<span data-ttu-id="fc563-118">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="fc563-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc563-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="fc563-119">Remarks</span></span>

<span data-ttu-id="fc563-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc563-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc563-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc563-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc563-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc563-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc563-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc563-123">Schema Name</span></span>  <br/> |<span data-ttu-id="fc563-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fc563-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc563-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc563-125">Validation File</span></span>  <br/> |<span data-ttu-id="fc563-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fc563-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc563-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc563-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc563-128">False</span><span class="sxs-lookup"><span data-stu-id="fc563-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc563-129">См. также</span><span class="sxs-lookup"><span data-stu-id="fc563-129">See also</span></span>

- [<span data-ttu-id="fc563-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fc563-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

