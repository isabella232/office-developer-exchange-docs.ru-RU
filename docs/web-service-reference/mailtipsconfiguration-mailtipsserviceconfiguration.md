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
ms.openlocfilehash: 9128ee99545066899c3b27b624f10a9f1bd36c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467790"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="6e7b6-103">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="6e7b6-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="6e7b6-104">Элемент **маилтипсконфигуратион** содержит сведения о конфигурации службы для почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
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

 <span data-ttu-id="6e7b6-105">**маилтипссервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="6e7b6-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e7b6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e7b6-106">Attributes and elements</span></span>

<span data-ttu-id="6e7b6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e7b6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e7b6-108">Attributes</span></span>

<span data-ttu-id="6e7b6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e7b6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e7b6-110">Child elements</span></span>

|<span data-ttu-id="6e7b6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e7b6-111">**Element**</span></span>|<span data-ttu-id="6e7b6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e7b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e7b6-113">маилтипсенаблед</span><span class="sxs-lookup"><span data-stu-id="6e7b6-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="6e7b6-114">Указывает, доступна ли служба советов по работе с почтой.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="6e7b6-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6e7b6-116">максреЦипиентспержетмаилтипсрекуест</span><span class="sxs-lookup"><span data-stu-id="6e7b6-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="6e7b6-117">Указывает максимальное количество получателей, которые могут быть переданы в операцию с помощью [подсказок](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6e7b6-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="6e7b6-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6e7b6-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="6e7b6-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="6e7b6-120">Представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="6e7b6-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6e7b6-122">ларжеаудиенцесрешолд</span><span class="sxs-lookup"><span data-stu-id="6e7b6-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="6e7b6-123">Представляет пороговое значение большой аудитории для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="6e7b6-124">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6e7b6-125">шовекстерналреЦипиенткаунт</span><span class="sxs-lookup"><span data-stu-id="6e7b6-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="6e7b6-126">Указывает, должны ли потребители [операции](getmailtips-operation.md) с подсказками отображать подсказки для почты, указывающие количество внешних получателей, на которые адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="6e7b6-127">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="6e7b6-128">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="6e7b6-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="6e7b6-129">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="6e7b6-130">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6e7b6-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e7b6-131">Parent elements</span></span>

|<span data-ttu-id="6e7b6-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e7b6-132">**Element**</span></span>|<span data-ttu-id="6e7b6-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e7b6-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e7b6-134">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="6e7b6-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="6e7b6-135">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e7b6-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6e7b6-136">Text value</span></span>

<span data-ttu-id="6e7b6-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e7b6-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="6e7b6-138">Remarks</span></span>

<span data-ttu-id="6e7b6-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e7b6-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e7b6-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e7b6-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e7b6-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e7b6-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e7b6-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e7b6-142">Schema Name</span></span>  <br/> |<span data-ttu-id="6e7b6-143">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6e7b6-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e7b6-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e7b6-144">Validation File</span></span>  <br/> |<span data-ttu-id="6e7b6-145">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6e7b6-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e7b6-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e7b6-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e7b6-147">False</span><span class="sxs-lookup"><span data-stu-id="6e7b6-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e7b6-148">См. также</span><span class="sxs-lookup"><span data-stu-id="6e7b6-148">See also</span></span>



- [<span data-ttu-id="6e7b6-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6e7b6-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

