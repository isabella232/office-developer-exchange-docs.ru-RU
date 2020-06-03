---
title: бккреЦипиент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BccRecipient
api_type:
- schema
ms.assetid: 4ef0cff5-8a5a-4d76-9d2b-938774d8fc1b
description: Элемент БккреЦипиент представляет получателя, который получает скрытую копию (BCC) сообщения электронной почты.
ms.openlocfilehash: 8296af1d74338bdfb1f4cb7bc7449ad91a9cd531
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461529"
---
# <a name="bccrecipient"></a><span data-ttu-id="a9945-103">бккреЦипиент</span><span class="sxs-lookup"><span data-stu-id="a9945-103">BccRecipient</span></span>

<span data-ttu-id="a9945-104">Элемент **бккреЦипиент** представляет получателя, который получает скрытую копию (BCC) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a9945-104">The **BccRecipient** element represents a recipient to receive a blind carbon copy (Bcc) of an e-mail message.</span></span> 
  
```XML
<BccRecipient>true | false</BccRecipient>
```

 <span data-ttu-id="a9945-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a9945-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a9945-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a9945-106">Attributes and elements</span></span>

<span data-ttu-id="a9945-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a9945-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a9945-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a9945-108">Attributes</span></span>

<span data-ttu-id="a9945-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a9945-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a9945-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a9945-110">Child elements</span></span>

<span data-ttu-id="a9945-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a9945-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a9945-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a9945-112">Parent elements</span></span>

|<span data-ttu-id="a9945-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a9945-113">**Element**</span></span>|<span data-ttu-id="a9945-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a9945-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a9945-115">реЦипиенттраккинжевент</span><span class="sxs-lookup"><span data-stu-id="a9945-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="a9945-116">Содержит сведения об отдельном событии получателя.</span><span class="sxs-lookup"><span data-stu-id="a9945-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a9945-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a9945-117">Text value</span></span>

<span data-ttu-id="a9945-118">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="a9945-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="a9945-119">Значение **true** указывает, что получатель является скрытой копии; значение **false** указывает, что получатель не является скрытой копии.</span><span class="sxs-lookup"><span data-stu-id="a9945-119">A value of **true** indicates that the recipient is blind carbon copied; a value of **false** indicates that the recipient is not blind carbon copied.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a9945-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="a9945-120">Remarks</span></span>

<span data-ttu-id="a9945-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a9945-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a9945-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a9945-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a9945-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a9945-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a9945-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a9945-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a9945-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a9945-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="a9945-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a9945-126">Validation File</span></span>  <br/> |<span data-ttu-id="a9945-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a9945-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a9945-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a9945-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a9945-129">False</span><span class="sxs-lookup"><span data-stu-id="a9945-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a9945-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a9945-130">See also</span></span>



- [<span data-ttu-id="a9945-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a9945-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

