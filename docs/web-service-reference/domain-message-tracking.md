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
ms.openlocfilehash: 77da9028766881b9bc633e1b3318cd4d70c6b72f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457027"
---
# <a name="domain-message-tracking"></a><span data-ttu-id="11ee5-103">Domain (отслеживание сообщений)</span><span class="sxs-lookup"><span data-stu-id="11ee5-103">Domain (Message Tracking)</span></span>

<span data-ttu-id="11ee5-104">Элемент **domain** представляет домен, который требуется найти.</span><span class="sxs-lookup"><span data-stu-id="11ee5-104">The **Domain** element represents the domain to search for.</span></span> 
  
```XML
<Domain/>
```

 <span data-ttu-id="11ee5-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="11ee5-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11ee5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11ee5-106">Attributes and elements</span></span>

<span data-ttu-id="11ee5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11ee5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11ee5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11ee5-108">Attributes</span></span>

<span data-ttu-id="11ee5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11ee5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11ee5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11ee5-110">Child elements</span></span>

<span data-ttu-id="11ee5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11ee5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11ee5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11ee5-112">Parent elements</span></span>

|<span data-ttu-id="11ee5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11ee5-113">**Element**</span></span>|<span data-ttu-id="11ee5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11ee5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11ee5-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="11ee5-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="11ee5-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="11ee5-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11ee5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="11ee5-117">Text value</span></span>

<span data-ttu-id="11ee5-118">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="11ee5-118">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="11ee5-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="11ee5-119">Remarks</span></span>

<span data-ttu-id="11ee5-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="11ee5-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11ee5-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11ee5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11ee5-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11ee5-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11ee5-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11ee5-123">Schema Name</span></span>  <br/> |<span data-ttu-id="11ee5-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="11ee5-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11ee5-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11ee5-125">Validation File</span></span>  <br/> |<span data-ttu-id="11ee5-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="11ee5-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11ee5-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11ee5-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="11ee5-128">False</span><span class="sxs-lookup"><span data-stu-id="11ee5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11ee5-129">См. также</span><span class="sxs-lookup"><span data-stu-id="11ee5-129">See also</span></span>

- [<span data-ttu-id="11ee5-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="11ee5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

