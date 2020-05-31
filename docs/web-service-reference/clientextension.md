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
ms.openlocfilehash: 5051248a2c8e664d82666bd7b42ee3c3046f43fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761684"
---
# <a name="clientextension"></a><span data-ttu-id="b6b2d-103">клиентекстенсион</span><span class="sxs-lookup"><span data-stu-id="b6b2d-103">ClientExtension</span></span>

<span data-ttu-id="b6b2d-104">Элемент **клиентекстенсион** содержит сведения о пользователе и конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-104">The **ClientExtension** element contains user and configuration information about an app.</span></span> 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 <span data-ttu-id="b6b2d-105">**клиентекстенсионтипе**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-105">**ClientExtensionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6b2d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b6b2d-106">Attributes and elements</span></span>

<span data-ttu-id="b6b2d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6b2d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b6b2d-108">Attributes</span></span>

|<span data-ttu-id="b6b2d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-109">**Attribute**</span></span>|<span data-ttu-id="b6b2d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6b2d-111">Доступный доступ</span><span class="sxs-lookup"><span data-stu-id="b6b2d-111">IsAvailable</span></span>  <br/> |<span data-ttu-id="b6b2d-112">Указывает, доступно ли приложение.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-112">Specifies whether the app is available.</span></span> <span data-ttu-id="b6b2d-113">Текстовое значение **true** для атрибута **Available** указывает на то, что приложение доступно.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-113">A text value of **true** for the **IsAvailable** attribute indicates that the app is available.</span></span> <span data-ttu-id="b6b2d-114">Значение **false** указывает, что приложение недоступно.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-114">A value of **false** indicates that the app is not available.</span></span> <span data-ttu-id="b6b2d-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-116">Обязательный</span><span class="sxs-lookup"><span data-stu-id="b6b2d-116">IsMandatory</span></span>  <br/> |<span data-ttu-id="b6b2d-117">Указывает, является ли приложение обязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-117">Specifies whether the app is mandatory.</span></span> <span data-ttu-id="b6b2d-118">Текстовое значение **true** **для атрибута InAttribute** указывает на то, что приложение является обязательным для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-118">A text value of **true** for the **IsMandatory** attribute indicates that the app is mandatory for the mailbox.</span></span> <span data-ttu-id="b6b2d-119">Значение **false** указывает, что приложение не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-119">A value of **false** indicates that the app is not mandatory.</span></span> <span data-ttu-id="b6b2d-120">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-120">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-121">исенабледбидефаулт</span><span class="sxs-lookup"><span data-stu-id="b6b2d-121">IsEnabledByDefault</span></span>  <br/> |<span data-ttu-id="b6b2d-122">Указывает, включено ли приложение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-122">Specifies whether the app is enabled by default.</span></span> <span data-ttu-id="b6b2d-123">Текстовое значение **true** для атрибута **исенабледбидефаулт** указывает, что приложение включено по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-123">A text value of **true** for the **IsEnabledByDefault** attribute indicates that the app is enabled by default.</span></span> <span data-ttu-id="b6b2d-124">Значение **false** указывает, что приложение по умолчанию отключено.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-124">A value of **false** indicates that the app is not enabled by default.</span></span> <span data-ttu-id="b6b2d-125">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-125">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-126">ProvidedTo</span><span class="sxs-lookup"><span data-stu-id="b6b2d-126">ProvidedTo</span></span>  <br/> |<span data-ttu-id="b6b2d-127">Указывает, кому предоставляется приложение.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-127">Specifies to whom the app is provided.</span></span> <span data-ttu-id="b6b2d-128">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-128">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-129">Тип</span><span class="sxs-lookup"><span data-stu-id="b6b2d-129">Type</span></span>  <br/> |<span data-ttu-id="b6b2d-130">Указывает тип приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-130">Specifies the type of the app.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-131">Scope</span><span class="sxs-lookup"><span data-stu-id="b6b2d-131">Scope</span></span>  <br/> |<span data-ttu-id="b6b2d-132">Указывает область приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-132">Specifies the scope of the app.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-133">маркетплацеассетид</span><span class="sxs-lookup"><span data-stu-id="b6b2d-133">MarketplaceAssetId</span></span>  <br/> |<span data-ttu-id="b6b2d-134">Указывает идентификатор ресурса Marketplace для приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-134">Specifies the marketplace asset identifier of the app.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-135">маркетплацеконтентмаркет</span><span class="sxs-lookup"><span data-stu-id="b6b2d-135">MarketplaceContentMarket</span></span>  <br/> |<span data-ttu-id="b6b2d-136">Указывает контент Marketplace, который видит пользователь для получения сведений и рецензирования приложения.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-136">Specifies the marketplace content that a user sees for details and reviews about an app.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-137">аппстатус</span><span class="sxs-lookup"><span data-stu-id="b6b2d-137">AppStatus</span></span>  <br/> |<span data-ttu-id="b6b2d-138">Указывает код состояния почтового приложения в неожиданном состоянии.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-138">Specifies the status code of a mail app in an unexpected state.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-139">етокен</span><span class="sxs-lookup"><span data-stu-id="b6b2d-139">Etoken</span></span>  <br/> |<span data-ttu-id="b6b2d-140">Указывает маркер лицензии для почтовых или пробных почтовых приложений.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-140">Specifies the license token for paid or trial mail apps.</span></span>  <br/> |
   
#### <a name="type"></a><span data-ttu-id="b6b2d-141">Тип</span><span class="sxs-lookup"><span data-stu-id="b6b2d-141">Type</span></span>

|<span data-ttu-id="b6b2d-142">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-142">**Value**</span></span>|<span data-ttu-id="b6b2d-143">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-143">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6b2d-144">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="b6b2d-144">Default</span></span>  <br/> |<span data-ttu-id="b6b2d-145">Указывает, что приложение доступно по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-145">Indicates that the app is available by default.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-146">Личные сведения</span><span class="sxs-lookup"><span data-stu-id="b6b2d-146">Private</span></span>  <br/> |<span data-ttu-id="b6b2d-147">Указывает, что приложение является частным.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-147">Indicates that the app is private.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-148">Рынках</span><span class="sxs-lookup"><span data-stu-id="b6b2d-148">MarketPlace</span></span>  <br/> |<span data-ttu-id="b6b2d-149">Указывает, что приложение является приложением Marketplace.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-149">Indicates that the app is a marketplace app.</span></span>  <br/> |
   
#### <a name="scope"></a><span data-ttu-id="b6b2d-150">Scope</span><span class="sxs-lookup"><span data-stu-id="b6b2d-150">Scope</span></span>

|<span data-ttu-id="b6b2d-151">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-151">**Value**</span></span>|<span data-ttu-id="b6b2d-152">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-152">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6b2d-153">Нет</span><span class="sxs-lookup"><span data-stu-id="b6b2d-153">None</span></span>  <br/> |<span data-ttu-id="b6b2d-154">Указывает, что в приложении нет области.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-154">Indicates that the app has no scope.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-155">User</span><span class="sxs-lookup"><span data-stu-id="b6b2d-155">User</span></span>  <br/> |<span data-ttu-id="b6b2d-156">Указывает, что приложение предназначено для каждого пользователя.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-156">Indicates that the app is per user.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-157">Организация</span><span class="sxs-lookup"><span data-stu-id="b6b2d-157">Organization</span></span>  <br/> |<span data-ttu-id="b6b2d-158">Указывает, что приложение предназначено для Организации.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-158">Indicates that the app is for an organization.</span></span>  <br/> |
|<span data-ttu-id="b6b2d-159">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="b6b2d-159">Default</span></span>  <br/> |<span data-ttu-id="b6b2d-160">Указывает, что приложение является приложением по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-160">Indicates that the app is a default app.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b6b2d-161">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b6b2d-161">Child elements</span></span>

|<span data-ttu-id="b6b2d-162">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-162">**Element**</span></span>|<span data-ttu-id="b6b2d-163">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6b2d-164">спеЦификусерс</span><span class="sxs-lookup"><span data-stu-id="b6b2d-164">SpecificUsers</span></span>](specificusers.md) <br/> |<span data-ttu-id="b6b2d-165">Указывает учетные записи электронной почты, которые могут получать доступ к приложению.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-165">Specifies the email accounts that can access the app.</span></span>  <br/> |
|[<span data-ttu-id="b6b2d-166">Манифест</span><span class="sxs-lookup"><span data-stu-id="b6b2d-166">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="b6b2d-167">Содержит файл манифеста приложения с кодировкой Base 64.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-167">Contains the base-64 encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b6b2d-168">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b6b2d-168">Parent elements</span></span>

|<span data-ttu-id="b6b2d-169">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-169">**Element**</span></span>|<span data-ttu-id="b6b2d-170">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b6b2d-170">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6b2d-171">клиентекстенсионс</span><span class="sxs-lookup"><span data-stu-id="b6b2d-171">ClientExtensions</span></span>](clientextensions.md) <br/> |<span data-ttu-id="b6b2d-172">Указывает массив элементов **клиентекстенсион** .</span><span class="sxs-lookup"><span data-stu-id="b6b2d-172">Specifies an array of **ClientExtension** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6b2d-173">Примечания</span><span class="sxs-lookup"><span data-stu-id="b6b2d-173">Remarks</span></span>

<span data-ttu-id="b6b2d-174">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-174">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b6b2d-175">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b6b2d-175">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6b2d-176">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b6b2d-176">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6b2d-177">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b6b2d-177">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6b2d-178">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b6b2d-178">Schema Name</span></span>  <br/> |<span data-ttu-id="b6b2d-179">Схема типа</span><span class="sxs-lookup"><span data-stu-id="b6b2d-179">Type schema</span></span>  <br/> |
|<span data-ttu-id="b6b2d-180">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b6b2d-180">Validation File</span></span>  <br/> |<span data-ttu-id="b6b2d-181">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b6b2d-181">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6b2d-182">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b6b2d-182">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b6b2d-183">См. также</span><span class="sxs-lookup"><span data-stu-id="b6b2d-183">See also</span></span>



- [<span data-ttu-id="b6b2d-184">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b6b2d-184">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

