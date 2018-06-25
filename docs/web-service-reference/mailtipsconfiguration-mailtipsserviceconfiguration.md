---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: Элемент MailTipsConfiguration содержит сведения о конфигурации службы для службы советы почты.
ms.openlocfilehash: ea92af3ebb2d2f720e5823c5317d09d5bcdb3978
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834321"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="0c193-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="0c193-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="0c193-104">Элемент **MailTipsConfiguration** содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="0c193-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 <span data-ttu-id="0c193-105">**MailTipsServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="0c193-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c193-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0c193-106">Attributes and elements</span></span>

<span data-ttu-id="0c193-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0c193-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c193-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0c193-108">Attributes</span></span>

<span data-ttu-id="0c193-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c193-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c193-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0c193-110">Child elements</span></span>

|<span data-ttu-id="0c193-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c193-111">**Element**</span></span>|<span data-ttu-id="0c193-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c193-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c193-113">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="0c193-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="0c193-114">Указывает, доступна ли служба советы почты.</span><span class="sxs-lookup"><span data-stu-id="0c193-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="0c193-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c193-116">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="0c193-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="0c193-117">Указывает максимальное количество получателей, которые могут передаваться [GetMailTips операции](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="0c193-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="0c193-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c193-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="0c193-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="0c193-120">Представляет максимальный размер сообщения, можно принять получателя.</span><span class="sxs-lookup"><span data-stu-id="0c193-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="0c193-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c193-122">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="0c193-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="0c193-123">Представляет большая аудитория пороговое значение для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c193-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="0c193-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c193-125">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="0c193-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="0c193-126">Указывает ли объекты-получатели [GetMailTips операции](getmailtips-operation.md) для отображения почтовые подсказки, которые указывают число внешних получателей, к которым адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="0c193-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="0c193-127">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0c193-128">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="0c193-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="0c193-129">Определяет список внутренних доменов SMTP организации.</span><span class="sxs-lookup"><span data-stu-id="0c193-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="0c193-130">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0c193-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c193-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0c193-131">Parent elements</span></span>

|<span data-ttu-id="0c193-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0c193-132">**Element**</span></span>|<span data-ttu-id="0c193-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c193-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c193-134">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="0c193-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="0c193-135">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="0c193-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0c193-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0c193-136">Text value</span></span>

<span data-ttu-id="0c193-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="0c193-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0c193-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="0c193-138">Remarks</span></span>

<span data-ttu-id="0c193-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0c193-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c193-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0c193-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c193-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0c193-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c193-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0c193-142">Schema Name</span></span>  <br/> |<span data-ttu-id="0c193-143">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0c193-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c193-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0c193-144">Validation File</span></span>  <br/> |<span data-ttu-id="0c193-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0c193-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c193-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0c193-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c193-147">False</span><span class="sxs-lookup"><span data-stu-id="0c193-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c193-148">См. также</span><span class="sxs-lookup"><span data-stu-id="0c193-148">See also</span></span>



- [<span data-ttu-id="0c193-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0c193-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

