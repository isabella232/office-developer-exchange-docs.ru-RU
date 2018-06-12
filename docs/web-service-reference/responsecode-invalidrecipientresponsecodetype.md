---
title: ResponseCode (InvalidRecipientResponseCodeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: Элемент ResponseCode предоставляет сведения о почему получатель является недопустимым.
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="c0017-103">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="c0017-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="c0017-104">Элемент **ResponseCode** предоставляет сведения о почему получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="c0017-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="c0017-105">**InvalidRecipientResponseCodeType**</span><span class="sxs-lookup"><span data-stu-id="c0017-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0017-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c0017-106">Attributes and elements</span></span>

<span data-ttu-id="c0017-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c0017-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0017-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c0017-108">Attributes</span></span>

<span data-ttu-id="c0017-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0017-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0017-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c0017-110">Child elements</span></span>

<span data-ttu-id="c0017-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0017-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0017-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c0017-112">Parent elements</span></span>

|<span data-ttu-id="c0017-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c0017-113">**Element**</span></span>|<span data-ttu-id="c0017-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0017-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0017-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="c0017-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="c0017-116">Содержит SMTP-адрес недопустимого получателя и сведения о почему получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="c0017-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0017-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c0017-117">Text value</span></span>

<span data-ttu-id="c0017-118">В следующей таблице приведены возможные значения для элемента **ResponseCode** .</span><span class="sxs-lookup"><span data-stu-id="c0017-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="c0017-119">**Код**</span><span class="sxs-lookup"><span data-stu-id="c0017-119">**Code**</span></span>|<span data-ttu-id="c0017-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0017-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0017-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="c0017-121">OtherError</span></span>  <br/> |<span data-ttu-id="c0017-122">Указывает, что ошибки не указан с другой код ошибки.</span><span class="sxs-lookup"><span data-stu-id="c0017-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="c0017-123">RecipientOrganizationNotFederated</span><span class="sxs-lookup"><span data-stu-id="c0017-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="c0017-124">Указывает, что отношение общего доступа не доступен с организацией, указанного в поле адрес электронной почты получателя SMTP.</span><span class="sxs-lookup"><span data-stu-id="c0017-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="c0017-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="c0017-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="c0017-126">Указывает, что возникла проблема получение маркера безопасности на основе сервера маркеров.</span><span class="sxs-lookup"><span data-stu-id="c0017-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="c0017-127">SystemPolicyBlocksSharingWithThisRecipient</span><span class="sxs-lookup"><span data-stu-id="c0017-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="c0017-128">Указывает, что системный администратор значение системной политики, который блокирует общий доступ для указанного получателя.</span><span class="sxs-lookup"><span data-stu-id="c0017-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="c0017-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="c0017-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="c0017-130">Указывает, что службы маркеров безопасности, используемый для указанного получателя неизвестно.</span><span class="sxs-lookup"><span data-stu-id="c0017-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0017-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="c0017-131">Remarks</span></span>

<span data-ttu-id="c0017-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0017-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0017-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c0017-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0017-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c0017-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0017-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c0017-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c0017-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c0017-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0017-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c0017-137">Validation File</span></span>  <br/> |<span data-ttu-id="c0017-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c0017-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0017-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c0017-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0017-140">False</span><span class="sxs-lookup"><span data-stu-id="c0017-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0017-141">См. также</span><span class="sxs-lookup"><span data-stu-id="c0017-141">See also</span></span>



[<span data-ttu-id="c0017-142">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="c0017-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="c0017-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c0017-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

