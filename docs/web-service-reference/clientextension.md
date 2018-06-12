---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: Элемент ClientExtension содержит пользователей и конфигурации сведения о приложении.
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761684"
---
# <a name="clientextension"></a><span data-ttu-id="0d17a-103">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="0d17a-103">ClientExtension</span></span>

<span data-ttu-id="0d17a-104">Элемент **ClientExtension** содержит пользователей и конфигурации сведения о приложении.</span><span class="sxs-lookup"><span data-stu-id="0d17a-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="0d17a-105">**ClientExtensionType**</span><span class="sxs-lookup"><span data-stu-id="0d17a-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d17a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d17a-106">Attributes and elements</span></span>

<span data-ttu-id="0d17a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0d17a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d17a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d17a-108">Attributes</span></span>

|<span data-ttu-id="0d17a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0d17a-109">**Attribute**</span></span>|<span data-ttu-id="0d17a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d17a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d17a-111">IsAvailable</span><span class="sxs-lookup"><span data-stu-id="0d17a-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="0d17a-112">Указывает, доступна ли приложение.</span><span class="sxs-lookup"><span data-stu-id="0d17a-112">Specifies whether the app is available.</span></span> <span data-ttu-id="0d17a-113">Текстовое значение **true** для атрибута **IsAvailable** указывает, что приложение доступно.</span><span class="sxs-lookup"><span data-stu-id="0d17a-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="0d17a-114">Значение **false** указывает, что приложение недоступно.</span><span class="sxs-lookup"><span data-stu-id="0d17a-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="0d17a-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="0d17a-116">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="0d17a-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="0d17a-117">Указывает, будет ли приложение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="0d17a-118">Текстовое значение **true** для атрибута **IsMandatory** указывает, что приложение является обязательным для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="0d17a-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="0d17a-119">Значение **false** указывает, что приложение не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="0d17a-120">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="0d17a-121">IsEnabledByDefault</span><span class="sxs-lookup"><span data-stu-id="0d17a-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="0d17a-122">Указывает, включена ли приложение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d17a-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="0d17a-123">Текстовое значение **true** для атрибута **IsEnabledByDefault** указывает, что приложение включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d17a-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="0d17a-124">Значение **false** указывает, что приложение не включен по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d17a-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="0d17a-125">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="0d17a-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="0d17a-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="0d17a-127">Указывает, к которому предоставляется приложения.</span><span class="sxs-lookup"><span data-stu-id="0d17a-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="0d17a-128">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d17a-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="0d17a-129">Тип</span><span class="sxs-lookup"><span data-stu-id="0d17a-129">Type</span></span>  <br/> |<span data-ttu-id="0d17a-130">Указывает тип приложения.</span><span class="sxs-lookup"><span data-stu-id="0d17a-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="0d17a-131">Область</span><span class="sxs-lookup"><span data-stu-id="0d17a-131">Scope</span></span>  <br/> |<span data-ttu-id="0d17a-132">Область приложения.</span><span class="sxs-lookup"><span data-stu-id="0d17a-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="0d17a-133">MarketplaceAssetId</span><span class="sxs-lookup"><span data-stu-id="0d17a-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="0d17a-134">Указывает идентификатор средств marketplace приложения.</span><span class="sxs-lookup"><span data-stu-id="0d17a-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="0d17a-135">MarketplaceContentMarket</span><span class="sxs-lookup"><span data-stu-id="0d17a-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="0d17a-136">Определяет содержимое marketplace, пользователь видит для получения дополнительных сведений и дается обзор о приложении.</span><span class="sxs-lookup"><span data-stu-id="0d17a-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="0d17a-137">AppStatus</span><span class="sxs-lookup"><span data-stu-id="0d17a-137">AppStatus</span></span>  <br/> |<span data-ttu-id="0d17a-138">Указывает код состояния почтового приложения в непредвиденное состояние.</span><span class="sxs-lookup"><span data-stu-id="0d17a-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="0d17a-139">Etoken</span><span class="sxs-lookup"><span data-stu-id="0d17a-139">Etoken</span></span>  <br/> |<span data-ttu-id="0d17a-140">Задает маркер лицензии платной или пробного почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="0d17a-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="0d17a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="0d17a-141">Type</span></span>

|<span data-ttu-id="0d17a-142">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d17a-142">**Value**</span></span>|<span data-ttu-id="0d17a-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d17a-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d17a-144">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="0d17a-144">Default</span></span>  <br/> |<span data-ttu-id="0d17a-145">Указывает, что приложение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d17a-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="0d17a-146">частная переменная</span><span class="sxs-lookup"><span data-stu-id="0d17a-146">Private</span></span>  <br/> |<span data-ttu-id="0d17a-147">Указывает, что приложение является частной.</span><span class="sxs-lookup"><span data-stu-id="0d17a-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="0d17a-148">Магазин</span><span class="sxs-lookup"><span data-stu-id="0d17a-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="0d17a-149">Указывает, что приложение является приложением marketplace.</span><span class="sxs-lookup"><span data-stu-id="0d17a-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="0d17a-150">Область</span><span class="sxs-lookup"><span data-stu-id="0d17a-150">Scope</span></span>

|<span data-ttu-id="0d17a-151">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d17a-151">**Value**</span></span>|<span data-ttu-id="0d17a-152">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d17a-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d17a-153">Нет</span><span class="sxs-lookup"><span data-stu-id="0d17a-153">None</span></span>  <br/> |<span data-ttu-id="0d17a-154">Указывает, что приложение не будет иметь область.</span><span class="sxs-lookup"><span data-stu-id="0d17a-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="0d17a-155">Пользователь</span><span class="sxs-lookup"><span data-stu-id="0d17a-155">User</span></span>  <br/> |<span data-ttu-id="0d17a-156">Указывает, что приложение на одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="0d17a-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="0d17a-157">Организация</span><span class="sxs-lookup"><span data-stu-id="0d17a-157">Organization</span></span>  <br/> |<span data-ttu-id="0d17a-158">Указывает, что приложение для организации.</span><span class="sxs-lookup"><span data-stu-id="0d17a-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="0d17a-159">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="0d17a-159">Default</span></span>  <br/> |<span data-ttu-id="0d17a-160">Указывает, что приложение является стандартным приложением.</span><span class="sxs-lookup"><span data-stu-id="0d17a-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0d17a-161">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d17a-161">Child elements</span></span>

|<span data-ttu-id="0d17a-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d17a-162">**Element**</span></span>|<span data-ttu-id="0d17a-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d17a-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d17a-164">SpecificUsers</span><span class="sxs-lookup"><span data-stu-id="0d17a-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="0d17a-165">Задает учетных записей электронной почты, которые могут получить доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="0d17a-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="0d17a-166">Манифест</span><span class="sxs-lookup"><span data-stu-id="0d17a-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="0d17a-167">Содержит файл манифеста приложения закодированный base-64.</span><span class="sxs-lookup"><span data-stu-id="0d17a-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d17a-168">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d17a-168">Parent elements</span></span>

|<span data-ttu-id="0d17a-169">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d17a-169">**Element**</span></span>|<span data-ttu-id="0d17a-170">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d17a-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d17a-171">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="0d17a-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="0d17a-172">Указывает массив элементов **ClientExtension** .</span><span class="sxs-lookup"><span data-stu-id="0d17a-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0d17a-173">Замечания</span><span class="sxs-lookup"><span data-stu-id="0d17a-173">Remarks</span></span>

<span data-ttu-id="0d17a-174">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0d17a-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0d17a-175">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d17a-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d17a-176">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d17a-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d17a-177">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d17a-177">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0d17a-178">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d17a-178">Schema Name</span></span>  <br/> |<span data-ttu-id="0d17a-179">Схема типа</span><span class="sxs-lookup"><span data-stu-id="0d17a-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="0d17a-180">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d17a-180">Validation File</span></span>  <br/> |<span data-ttu-id="0d17a-181">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0d17a-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0d17a-182">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d17a-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="0d17a-183">См. также</span><span class="sxs-lookup"><span data-stu-id="0d17a-183">See also</span></span>



- [<span data-ttu-id="0d17a-184">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0d17a-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

