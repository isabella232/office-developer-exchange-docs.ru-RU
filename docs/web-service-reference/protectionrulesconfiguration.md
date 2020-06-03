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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456774"
---
# <a name="protectionrulesconfiguration"></a><span data-ttu-id="9f105-103">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="9f105-103">ProtectionRulesConfiguration</span></span>

<span data-ttu-id="9f105-104">Элемент **протектионрулесконфигуратион** содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="9f105-104">The **ProtectionRulesConfiguration** element contains service configuration information for the protection rules service.</span></span> 
  
```XML
<ProtectionRulesConfiguration RefreshInterval="">
   <Rules/>
   <InternalDomains/>
</ProtectionRulesConfiguration>
```

 <span data-ttu-id="9f105-105">**протектионрулессервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="9f105-105">**ProtectionRulesServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9f105-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9f105-106">Attributes and elements</span></span>

<span data-ttu-id="9f105-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9f105-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f105-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9f105-108">Attributes</span></span>

|<span data-ttu-id="9f105-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9f105-109">**Attribute**</span></span>|<span data-ttu-id="9f105-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f105-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f105-111">**RefreshInterval**</span><span class="sxs-lookup"><span data-stu-id="9f105-111">**RefreshInterval**</span></span> <br/> |<span data-ttu-id="9f105-112">Указывает, как часто клиент должен запрашивать правила защиты от сервера в течение всего времени.</span><span class="sxs-lookup"><span data-stu-id="9f105-112">Specifies how often, in whole hours, the client should request protection rules from the server.</span></span> <span data-ttu-id="9f105-113">Этот атрибут является обязательным, а его значение должно быть целым числом, равным или большим 1.</span><span class="sxs-lookup"><span data-stu-id="9f105-113">This attribute is required and its value must be an integer that is equal to or greater than 1.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f105-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9f105-114">Child elements</span></span>

|<span data-ttu-id="9f105-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f105-115">**Element**</span></span>|<span data-ttu-id="9f105-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f105-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f105-117">Условия</span><span class="sxs-lookup"><span data-stu-id="9f105-117">Rules </span></span>](rules-ex15websvcsotherref.md) <br/> |<span data-ttu-id="9f105-118">Массив правил защиты.</span><span class="sxs-lookup"><span data-stu-id="9f105-118">An array of protection rules.</span></span> <span data-ttu-id="9f105-119">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f105-119">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="9f105-120">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="9f105-120">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="9f105-121">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="9f105-121">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="9f105-122">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="9f105-122">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f105-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9f105-123">Parent elements</span></span>

|<span data-ttu-id="9f105-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9f105-124">**Element**</span></span>|<span data-ttu-id="9f105-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9f105-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f105-126">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="9f105-126">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="9f105-127">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="9f105-127">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9f105-128">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9f105-128">Text value</span></span>

<span data-ttu-id="9f105-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="9f105-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9f105-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="9f105-130">Remarks</span></span>

<span data-ttu-id="9f105-131">Конфигурация службы правил защиты состоит из списка правил, внутренних доменов и интервалов обновления.</span><span class="sxs-lookup"><span data-stu-id="9f105-131">The protection rules service configuration is comprised of a list of rules, internal domains, and a refresh interval.</span></span>
  
<span data-ttu-id="9f105-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9f105-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f105-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9f105-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f105-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9f105-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9f105-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9f105-135">Schema Name</span></span>  <br/> |<span data-ttu-id="9f105-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9f105-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9f105-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9f105-137">Validation File</span></span>  <br/> |<span data-ttu-id="9f105-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="9f105-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9f105-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9f105-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f105-140">False</span><span class="sxs-lookup"><span data-stu-id="9f105-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f105-141">См. также</span><span class="sxs-lookup"><span data-stu-id="9f105-141">See also</span></span>



- [<span data-ttu-id="9f105-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9f105-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

