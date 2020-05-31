---
title: инвалидреЦипиент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 9e2d3433-22d7-444b-9883-e5649297d8fe
description: Элемент ИнвалидреЦипиент содержит SMTP-адрес недопустимого получателя и сведения о том, почему получатель не является допустимым.
ms.openlocfilehash: 800056666e486e9337dcd1c2786f7e6db1e060bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833961"
---
# <a name="invalidrecipient"></a><span data-ttu-id="f0758-103">инвалидреЦипиент</span><span class="sxs-lookup"><span data-stu-id="f0758-103">InvalidRecipient</span></span>

<span data-ttu-id="f0758-104">Элемент **инвалидреЦипиент** содержит SMTP-адрес недопустимого получателя и сведения о том, почему получатель не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="f0758-104">The **InvalidRecipient** element contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>
   <SmtpAddress/>
   <ResponseCode/>
   <MessageText/>
</InvalidRecipient>

```

 <span data-ttu-id="f0758-105">**инвалидреЦипиенттипе**</span><span class="sxs-lookup"><span data-stu-id="f0758-105">**InvalidRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0758-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0758-106">Attributes and elements</span></span>

<span data-ttu-id="f0758-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f0758-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0758-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0758-108">Attributes</span></span>

<span data-ttu-id="f0758-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0758-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0758-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0758-110">Child elements</span></span>

|<span data-ttu-id="f0758-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0758-111">**Element**</span></span>|<span data-ttu-id="f0758-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0758-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0758-113">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="f0758-113">SmtpAddress</span></span>](smtpaddress.md) <br/> |<span data-ttu-id="f0758-114">Содержит SMTP-адрес недопустимого получателя.</span><span class="sxs-lookup"><span data-stu-id="f0758-114">Contains the SMTP address of the invalid recipient.</span></span> <span data-ttu-id="f0758-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0758-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="f0758-116">Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)</span><span class="sxs-lookup"><span data-stu-id="f0758-116">ResponseCode (InvalidRecipientResponseCodeType)</span></span>](responsecode-invalidrecipientresponsecodetype.md) <br/> |<span data-ttu-id="f0758-117">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="f0758-117">Provides an error code that identifies the specific error that the request encountered.</span></span> <span data-ttu-id="f0758-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="f0758-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="f0758-119">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="f0758-119">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f0758-120">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="f0758-120">Provides a text description of the status of the response.</span></span> <span data-ttu-id="f0758-121">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f0758-121">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0758-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0758-122">Parent elements</span></span>

|<span data-ttu-id="f0758-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0758-123">**Element**</span></span>|<span data-ttu-id="f0758-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0758-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0758-125">инвалидреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="f0758-125">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="f0758-126">Представляет недопустимые получатели запроса на общий доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="f0758-126">Represents the recipients of a folder sharing request that are invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0758-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="f0758-127">Remarks</span></span>

<span data-ttu-id="f0758-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0758-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0758-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0758-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0758-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0758-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0758-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0758-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f0758-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f0758-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0758-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0758-133">Validation File</span></span>  <br/> |<span data-ttu-id="f0758-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f0758-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0758-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0758-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0758-136">False</span><span class="sxs-lookup"><span data-stu-id="f0758-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0758-137">См. также</span><span class="sxs-lookup"><span data-stu-id="f0758-137">See also</span></span>



[<span data-ttu-id="f0758-138">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="f0758-138">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="f0758-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f0758-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

