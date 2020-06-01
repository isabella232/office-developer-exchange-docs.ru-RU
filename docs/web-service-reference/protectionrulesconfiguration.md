---
title: протектионрулесконфигуратион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProtectionRulesConfiguration
api_type:
- schema
ms.assetid: e5b4699a-476e-4053-bb52-873eb921c046
description: Элемент Протектионрулесконфигуратион содержит сведения о конфигурации службы для службы правил защиты.
ms.openlocfilehash: e664fba78f170c9f4c59b49b3a08c0dd2e4ed4cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456774"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="12bc0-103">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="12bc0-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="12bc0-104">Элемент **протектионрулесконфигуратион** содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="12bc0-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="12bc0-105">**протектионрулессервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="12bc0-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12bc0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="12bc0-106">Attributes and elements</span></span>

<span data-ttu-id="12bc0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="12bc0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12bc0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="12bc0-108">Attributes</span></span>

|<span data-ttu-id="12bc0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="12bc0-109">**Attribute**</span></span>|<span data-ttu-id="12bc0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12bc0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="12bc0-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="12bc0-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="12bc0-112">Указывает, как часто клиент должен запрашивать правила защиты от сервера в течение всего времени.</span><span class="sxs-lookup"><span data-stu-id="12bc0-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="12bc0-113">Этот атрибут является обязательным, а его значение должно быть целым числом, равным или большим 1.</span><span class="sxs-lookup"><span data-stu-id="12bc0-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="12bc0-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="12bc0-114">Child elements</span></span>

|<span data-ttu-id="12bc0-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12bc0-115">**Element**</span></span>|<span data-ttu-id="12bc0-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12bc0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bc0-117">Условия</span><span class="sxs-lookup"><span data-stu-id="12bc0-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="12bc0-118">Массив правил защиты.</span><span class="sxs-lookup"><span data-stu-id="12bc0-118">An array of protection rules.</span></span> <span data-ttu-id="12bc0-119">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="12bc0-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="12bc0-120">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="12bc0-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="12bc0-121">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="12bc0-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="12bc0-122">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="12bc0-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="12bc0-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="12bc0-123">Parent elements</span></span>

|<span data-ttu-id="12bc0-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12bc0-124">**Element**</span></span>|<span data-ttu-id="12bc0-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12bc0-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12bc0-126">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="12bc0-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="12bc0-127">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="12bc0-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12bc0-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="12bc0-128">Text value</span></span>

<span data-ttu-id="12bc0-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="12bc0-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12bc0-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="12bc0-130">Remarks</span></span>

<span data-ttu-id="12bc0-131">Конфигурация службы правил защиты состоит из списка правил, внутренних доменов и интервалов обновления.</span><span class="sxs-lookup"><span data-stu-id="12bc0-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="12bc0-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="12bc0-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12bc0-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="12bc0-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12bc0-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="12bc0-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="12bc0-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="12bc0-135">Schema Name</span></span>  <br/> |<span data-ttu-id="12bc0-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="12bc0-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="12bc0-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="12bc0-137">Validation File</span></span>  <br/> |<span data-ttu-id="12bc0-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="12bc0-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="12bc0-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="12bc0-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="12bc0-140">False</span><span class="sxs-lookup"><span data-stu-id="12bc0-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12bc0-141">См. также</span><span class="sxs-lookup"><span data-stu-id="12bc0-141">See also</span></span>



- [<span data-ttu-id="12bc0-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="12bc0-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

