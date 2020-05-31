---
title: Маилтипсконфигуратион (Маилтипссервицеконфигуратион)
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
description: Элемент Маилтипсконфигуратион содержит сведения о конфигурации службы для почтовых подсказок.
ms.openlocfilehash: ea92af3ebb2d2f720e5823c5317d09d5bcdb3978
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834321"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="2f60b-103">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="2f60b-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="2f60b-104">Элемент **маилтипсконфигуратион** содержит сведения о конфигурации службы для почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="2f60b-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
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

 <span data-ttu-id="2f60b-105">**маилтипссервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="2f60b-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f60b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2f60b-106">Attributes and elements</span></span>

<span data-ttu-id="2f60b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2f60b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f60b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2f60b-108">Attributes</span></span>

<span data-ttu-id="2f60b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2f60b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f60b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2f60b-110">Child elements</span></span>

|<span data-ttu-id="2f60b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f60b-111">**Element**</span></span>|<span data-ttu-id="2f60b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f60b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f60b-113">маилтипсенаблед</span><span class="sxs-lookup"><span data-stu-id="2f60b-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="2f60b-114">Указывает, доступна ли служба советов по работе с почтой.</span><span class="sxs-lookup"><span data-stu-id="2f60b-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="2f60b-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2f60b-116">максреЦипиентспержетмаилтипсрекуест</span><span class="sxs-lookup"><span data-stu-id="2f60b-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="2f60b-117">Указывает максимальное количество получателей, которые могут быть переданы в операцию с помощью [подсказок](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="2f60b-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="2f60b-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2f60b-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="2f60b-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="2f60b-120">Представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="2f60b-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="2f60b-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2f60b-122">ларжеаудиенцесрешолд</span><span class="sxs-lookup"><span data-stu-id="2f60b-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="2f60b-123">Представляет пороговое значение большой аудитории для клиента.</span><span class="sxs-lookup"><span data-stu-id="2f60b-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="2f60b-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2f60b-125">шовекстерналреЦипиенткаунт</span><span class="sxs-lookup"><span data-stu-id="2f60b-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="2f60b-126">Указывает, должны ли потребители [операции](getmailtips-operation.md) с подсказками отображать подсказки для почты, указывающие количество внешних получателей, на которые адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="2f60b-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="2f60b-127">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="2f60b-128">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="2f60b-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="2f60b-129">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="2f60b-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="2f60b-130">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="2f60b-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2f60b-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2f60b-131">Parent elements</span></span>

|<span data-ttu-id="2f60b-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2f60b-132">**Element**</span></span>|<span data-ttu-id="2f60b-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2f60b-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f60b-134">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="2f60b-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="2f60b-135">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="2f60b-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f60b-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2f60b-136">Text value</span></span>

<span data-ttu-id="2f60b-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="2f60b-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f60b-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="2f60b-138">Remarks</span></span>

<span data-ttu-id="2f60b-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2f60b-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f60b-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2f60b-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f60b-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2f60b-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2f60b-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2f60b-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2f60b-143">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="2f60b-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2f60b-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2f60b-144">Validation File</span></span>  <br/> |<span data-ttu-id="2f60b-145">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2f60b-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2f60b-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2f60b-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2f60b-147">False</span><span class="sxs-lookup"><span data-stu-id="2f60b-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f60b-148">См. также</span><span class="sxs-lookup"><span data-stu-id="2f60b-148">See also</span></span>



- [<span data-ttu-id="2f60b-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2f60b-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

