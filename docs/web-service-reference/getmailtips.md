---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: Элемент GetMailTips представляет получателей и типы почтовые подсказки для извлечения.
ms.openlocfilehash: aad3b3d9dd578d0c92bf7d48ee8b78b58c63e23d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762843"
---
# <a name="getmailtips"></a><span data-ttu-id="bd58c-103">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="bd58c-103">GetMailTips</span></span>

<span data-ttu-id="bd58c-104">Элемент **GetMailTips** представляет получателей и типы почтовые подсказки для извлечения.</span><span class="sxs-lookup"><span data-stu-id="bd58c-104">The **GetMailTips** element represents the recipients and types of mail tips to retrieve.</span></span> 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 <span data-ttu-id="bd58c-105">**GetMailTipsType**</span><span class="sxs-lookup"><span data-stu-id="bd58c-105">**GetMailTipsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd58c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd58c-106">Attributes and elements</span></span>

<span data-ttu-id="bd58c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bd58c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd58c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd58c-108">Attributes</span></span>

<span data-ttu-id="bd58c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd58c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd58c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd58c-110">Child elements</span></span>

|<span data-ttu-id="bd58c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd58c-111">**Element**</span></span>|<span data-ttu-id="bd58c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd58c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd58c-113">SendingAs</span><span class="sxs-lookup"><span data-stu-id="bd58c-113">SendingAs</span></span>](sendingas.md) <br/> |<span data-ttu-id="bd58c-114">Содержит адрес электронной почты, который пользователь пытается отправить как.</span><span class="sxs-lookup"><span data-stu-id="bd58c-114">Contains an e-mail address that a user is trying to send as.</span></span>  <br/> |
|[<span data-ttu-id="bd58c-115">Получатели (ArrayOfRecipientsType)</span><span class="sxs-lookup"><span data-stu-id="bd58c-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="bd58c-116">Содержит список получателей на наличие почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="bd58c-116">Contains a list of recipients to check for mail tips.</span></span>  <br/> |
|[<span data-ttu-id="bd58c-117">MailTipsRequested</span><span class="sxs-lookup"><span data-stu-id="bd58c-117">MailTipsRequested</span></span>](mailtipsrequested.md) <br/> |<span data-ttu-id="bd58c-118">Содержит типы, запрашивается из службы почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="bd58c-118">Contains the types of mail tips requested from the service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd58c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd58c-119">Parent elements</span></span>

<span data-ttu-id="bd58c-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd58c-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bd58c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bd58c-121">Text value</span></span>

<span data-ttu-id="bd58c-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd58c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd58c-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="bd58c-123">Remarks</span></span>

<span data-ttu-id="bd58c-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd58c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd58c-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd58c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd58c-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd58c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd58c-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd58c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bd58c-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bd58c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd58c-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd58c-129">Validation File</span></span>  <br/> |<span data-ttu-id="bd58c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bd58c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd58c-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd58c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd58c-132">False</span><span class="sxs-lookup"><span data-stu-id="bd58c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd58c-133">См. также</span><span class="sxs-lookup"><span data-stu-id="bd58c-133">See also</span></span>



- [<span data-ttu-id="bd58c-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd58c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

