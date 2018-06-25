---
title: InternalDomains (SmtpDomainList)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalDomains
api_type:
- schema
ms.assetid: 0f2cbb05-338d-4302-8871-a06e78b33f98
description: Элемент InternalDomains определяет список внутренних доменов SMTP организации.
ms.openlocfilehash: f37a31f4348a7eb0024656489f249dec349bc67b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833953"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="28764-103">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="28764-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="28764-104">Элемент **InternalDomains** определяет список внутренних доменов SMTP организации.</span><span class="sxs-lookup"><span data-stu-id="28764-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="28764-105">**SmtpDomainList**</span><span class="sxs-lookup"><span data-stu-id="28764-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28764-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28764-106">Attributes and elements</span></span>

<span data-ttu-id="28764-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="28764-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28764-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28764-108">Attributes</span></span>

<span data-ttu-id="28764-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28764-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28764-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28764-110">Child elements</span></span>

|<span data-ttu-id="28764-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28764-111">**Element**</span></span>|<span data-ttu-id="28764-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28764-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28764-113">Domain</span><span class="sxs-lookup"><span data-stu-id="28764-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="28764-114">Идентифицирует одного домена SMTP.</span><span class="sxs-lookup"><span data-stu-id="28764-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28764-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28764-115">Parent elements</span></span>

|<span data-ttu-id="28764-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28764-116">**Element**</span></span>|<span data-ttu-id="28764-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28764-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28764-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="28764-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="28764-119">Содержит сведения о конфигурации службы для службы советы почты.</span><span class="sxs-lookup"><span data-stu-id="28764-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="28764-120">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="28764-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="28764-121">Содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="28764-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28764-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28764-122">Text value</span></span>

<span data-ttu-id="28764-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="28764-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28764-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="28764-124">Remarks</span></span>

<span data-ttu-id="28764-125">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="28764-125">This element is required.</span></span> 
  
<span data-ttu-id="28764-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="28764-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28764-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28764-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28764-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28764-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="28764-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28764-129">Schema Name</span></span>  <br/> |<span data-ttu-id="28764-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="28764-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="28764-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28764-131">Validation File</span></span>  <br/> |<span data-ttu-id="28764-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="28764-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="28764-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28764-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="28764-134">False</span><span class="sxs-lookup"><span data-stu-id="28764-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28764-135">См. также</span><span class="sxs-lookup"><span data-stu-id="28764-135">See also</span></span>



- [<span data-ttu-id="28764-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="28764-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

