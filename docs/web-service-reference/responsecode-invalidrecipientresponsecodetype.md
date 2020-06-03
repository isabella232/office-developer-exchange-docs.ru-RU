---
title: Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)
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
description: Элемент Респонсекоде предоставляет сведения о причине неправильного получателя.
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529723"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="cdf7f-103">Респонсекоде (ИнвалидреЦипиентреспонсекодетипе)</span><span class="sxs-lookup"><span data-stu-id="cdf7f-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="cdf7f-104">Элемент **респонсекоде** предоставляет сведения о причине неправильного получателя.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="cdf7f-105">**инвалидреЦипиентреспонсекодетипе**</span><span class="sxs-lookup"><span data-stu-id="cdf7f-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cdf7f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cdf7f-106">Attributes and elements</span></span>

<span data-ttu-id="cdf7f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdf7f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cdf7f-108">Attributes</span></span>

<span data-ttu-id="cdf7f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdf7f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cdf7f-110">Child elements</span></span>

<span data-ttu-id="cdf7f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cdf7f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cdf7f-112">Parent elements</span></span>

|<span data-ttu-id="cdf7f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cdf7f-113">**Element**</span></span>|<span data-ttu-id="cdf7f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cdf7f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdf7f-115">инвалидреЦипиент</span><span class="sxs-lookup"><span data-stu-id="cdf7f-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="cdf7f-116">Содержит SMTP-адрес недопустимого получателя и сведения о почему получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cdf7f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cdf7f-117">Text value</span></span>

<span data-ttu-id="cdf7f-118">В следующей таблице приведены возможные значения для элемента **респонсекоде** .</span><span class="sxs-lookup"><span data-stu-id="cdf7f-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="cdf7f-119">**Code**</span><span class="sxs-lookup"><span data-stu-id="cdf7f-119">**Code**</span></span>|<span data-ttu-id="cdf7f-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cdf7f-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cdf7f-121">осереррор</span><span class="sxs-lookup"><span data-stu-id="cdf7f-121">OtherError</span></span>  <br/> |<span data-ttu-id="cdf7f-122">Указывает на то, что ошибка не указана другим кодом ответа на сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="cdf7f-123">реЦипиенторганизатионнотфедератед</span><span class="sxs-lookup"><span data-stu-id="cdf7f-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="cdf7f-124">Указывает, что отношение общего доступа недоступно в Организации, указанной в SMTP-адресе электронной почты получателя.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="cdf7f-125">каннотобтаинтокенфромстс</span><span class="sxs-lookup"><span data-stu-id="cdf7f-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="cdf7f-126">Указывает, что при получении маркера безопасности от сервера маркеров возникла проблема.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="cdf7f-127">системполициблокксшарингвиссисреЦипиент</span><span class="sxs-lookup"><span data-stu-id="cdf7f-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="cdf7f-128">Указывает, что системный администратор установил системную политику, которая блокирует общий доступ для указанного получателя.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="cdf7f-129">реЦипиенторганизатионфедератедвисункновнтокениссуер</span><span class="sxs-lookup"><span data-stu-id="cdf7f-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="cdf7f-130">Указывает, что служба безопасного токена, используемая указанным получателем, неизвестна.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cdf7f-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="cdf7f-131">Remarks</span></span>

<span data-ttu-id="cdf7f-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cdf7f-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdf7f-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cdf7f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdf7f-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cdf7f-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cdf7f-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cdf7f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="cdf7f-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cdf7f-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="cdf7f-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cdf7f-137">Validation File</span></span>  <br/> |<span data-ttu-id="cdf7f-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cdf7f-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cdf7f-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cdf7f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="cdf7f-140">False</span><span class="sxs-lookup"><span data-stu-id="cdf7f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cdf7f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="cdf7f-141">See also</span></span>



[<span data-ttu-id="cdf7f-142">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="cdf7f-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="cdf7f-143">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cdf7f-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

