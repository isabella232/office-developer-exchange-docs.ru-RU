---
title: клиентекстенсион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: Элемент Клиентекстенсион содержит сведения о пользователе и конфигурации приложения.
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460199"
---
# <a name="clientextension"></a><span data-ttu-id="bba15-103">клиентекстенсион</span><span class="sxs-lookup"><span data-stu-id="bba15-103">ClientExtension</span></span>

<span data-ttu-id="bba15-104">Элемент **клиентекстенсион** содержит сведения о пользователе и конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="bba15-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="bba15-105">**клиентекстенсионтипе**</span><span class="sxs-lookup"><span data-stu-id="bba15-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bba15-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bba15-106">Attributes and elements</span></span>

<span data-ttu-id="bba15-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bba15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bba15-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bba15-108">Attributes</span></span>

|<span data-ttu-id="bba15-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bba15-109">**Attribute**</span></span>|<span data-ttu-id="bba15-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba15-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bba15-111">Доступный доступ</span><span class="sxs-lookup"><span data-stu-id="bba15-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="bba15-112">Указывает, доступно ли приложение.</span><span class="sxs-lookup"><span data-stu-id="bba15-112">Specifies whether the app is available.</span></span> <span data-ttu-id="bba15-113">Текстовое значение **true** для атрибута **Available** указывает на то, что приложение доступно.</span><span class="sxs-lookup"><span data-stu-id="bba15-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="bba15-114">Значение **false** указывает, что приложение недоступно.</span><span class="sxs-lookup"><span data-stu-id="bba15-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="bba15-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="bba15-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="bba15-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="bba15-117">Указывает, является ли приложение обязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="bba15-118">Текстовое значение **true** **для атрибута InAttribute** указывает на то, что приложение является обязательным для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bba15-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="bba15-119">Значение **false** указывает, что приложение не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="bba15-120">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="bba15-121">исенабледбидефаулт</span><span class="sxs-lookup"><span data-stu-id="bba15-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="bba15-122">Указывает, включено ли приложение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bba15-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="bba15-123">Текстовое значение **true** для атрибута **исенабледбидефаулт** указывает, что приложение включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bba15-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="bba15-124">Значение **false** указывает, что приложение по умолчанию отключено.</span><span class="sxs-lookup"><span data-stu-id="bba15-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="bba15-125">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="bba15-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="bba15-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="bba15-127">Указывает, кому предоставляется приложение.</span><span class="sxs-lookup"><span data-stu-id="bba15-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="bba15-128">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bba15-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="bba15-129">Тип</span><span class="sxs-lookup"><span data-stu-id="bba15-129">Type</span></span>  <br/> |<span data-ttu-id="bba15-130">Указывает тип приложения.</span><span class="sxs-lookup"><span data-stu-id="bba15-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="bba15-131">Область</span><span class="sxs-lookup"><span data-stu-id="bba15-131">Scope</span></span>  <br/> |<span data-ttu-id="bba15-132">Указывает область приложения.</span><span class="sxs-lookup"><span data-stu-id="bba15-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="bba15-133">маркетплацеассетид</span><span class="sxs-lookup"><span data-stu-id="bba15-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="bba15-134">Указывает идентификатор ресурса Marketplace для приложения.</span><span class="sxs-lookup"><span data-stu-id="bba15-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="bba15-135">маркетплацеконтентмаркет</span><span class="sxs-lookup"><span data-stu-id="bba15-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="bba15-136">Указывает контент Marketplace, который видит пользователь для получения сведений и рецензирования приложения.</span><span class="sxs-lookup"><span data-stu-id="bba15-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="bba15-137">аппстатус</span><span class="sxs-lookup"><span data-stu-id="bba15-137">AppStatus</span></span>  <br/> |<span data-ttu-id="bba15-138">Указывает код состояния почтового приложения в неожиданном состоянии.</span><span class="sxs-lookup"><span data-stu-id="bba15-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="bba15-139">етокен</span><span class="sxs-lookup"><span data-stu-id="bba15-139">Etoken</span></span>  <br/> |<span data-ttu-id="bba15-140">Указывает маркер лицензии для почтовых или пробных почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="bba15-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="bba15-141">Тип</span><span class="sxs-lookup"><span data-stu-id="bba15-141">Type</span></span>

|<span data-ttu-id="bba15-142">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bba15-142">**Value**</span></span>|<span data-ttu-id="bba15-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba15-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bba15-144">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="bba15-144">Default</span></span>  <br/> |<span data-ttu-id="bba15-145">Указывает, что приложение доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bba15-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="bba15-146">Частный</span><span class="sxs-lookup"><span data-stu-id="bba15-146">Private</span></span>  <br/> |<span data-ttu-id="bba15-147">Указывает, что приложение является частным.</span><span class="sxs-lookup"><span data-stu-id="bba15-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="bba15-148">Рынках</span><span class="sxs-lookup"><span data-stu-id="bba15-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="bba15-149">Указывает, что приложение является приложением Marketplace.</span><span class="sxs-lookup"><span data-stu-id="bba15-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="bba15-150">Область</span><span class="sxs-lookup"><span data-stu-id="bba15-150">Scope</span></span>

|<span data-ttu-id="bba15-151">**Значение**</span><span class="sxs-lookup"><span data-stu-id="bba15-151">**Value**</span></span>|<span data-ttu-id="bba15-152">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba15-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bba15-153">Нет</span><span class="sxs-lookup"><span data-stu-id="bba15-153">None</span></span>  <br/> |<span data-ttu-id="bba15-154">Указывает, что в приложении нет области.</span><span class="sxs-lookup"><span data-stu-id="bba15-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="bba15-155">User</span><span class="sxs-lookup"><span data-stu-id="bba15-155">User</span></span>  <br/> |<span data-ttu-id="bba15-156">Указывает, что приложение предназначено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="bba15-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="bba15-157">Организация</span><span class="sxs-lookup"><span data-stu-id="bba15-157">Organization</span></span>  <br/> |<span data-ttu-id="bba15-158">Указывает, что приложение предназначено для Организации.</span><span class="sxs-lookup"><span data-stu-id="bba15-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="bba15-159">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="bba15-159">Default</span></span>  <br/> |<span data-ttu-id="bba15-160">Указывает, что приложение является приложением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="bba15-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bba15-161">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bba15-161">Child elements</span></span>

|<span data-ttu-id="bba15-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bba15-162">**Element**</span></span>|<span data-ttu-id="bba15-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba15-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bba15-164">спеЦификусерс</span><span class="sxs-lookup"><span data-stu-id="bba15-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="bba15-165">Указывает учетные записи электронной почты, которые могут получать доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="bba15-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="bba15-166">Манифест</span><span class="sxs-lookup"><span data-stu-id="bba15-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="bba15-167">Содержит файл манифеста приложения с кодировкой Base 64.</span><span class="sxs-lookup"><span data-stu-id="bba15-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bba15-168">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bba15-168">Parent elements</span></span>

|<span data-ttu-id="bba15-169">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bba15-169">**Element**</span></span>|<span data-ttu-id="bba15-170">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bba15-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bba15-171">клиентекстенсионс</span><span class="sxs-lookup"><span data-stu-id="bba15-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="bba15-172">Указывает массив элементов **клиентекстенсион** .</span><span class="sxs-lookup"><span data-stu-id="bba15-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bba15-173">Примечания</span><span class="sxs-lookup"><span data-stu-id="bba15-173">Remarks</span></span>

<span data-ttu-id="bba15-174">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bba15-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bba15-175">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bba15-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bba15-176">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bba15-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bba15-177">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bba15-177">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bba15-178">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bba15-178">Schema Name</span></span>  <br/> |<span data-ttu-id="bba15-179">Схема типа</span><span class="sxs-lookup"><span data-stu-id="bba15-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="bba15-180">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bba15-180">Validation File</span></span>  <br/> |<span data-ttu-id="bba15-181">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bba15-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bba15-182">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bba15-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bba15-183">См. также</span><span class="sxs-lookup"><span data-stu-id="bba15-183">See also</span></span>



- [<span data-ttu-id="bba15-184">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bba15-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

