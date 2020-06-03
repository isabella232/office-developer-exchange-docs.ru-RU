---
title: Имена внутренних доменов (Смтпдомаинлист)
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
description: Элемент имена внутренних доменов определяет список внутренних доменов SMTP Организации.
ms.openlocfilehash: ec7ef2d72ae922c751f8f50b72ff7d6b31b212ca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459968"
---
# <a name="internaldomains-smtpdomainlist"></a><span data-ttu-id="c870d-103">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="c870d-103">InternalDomains (SmtpDomainList)</span></span>

<span data-ttu-id="c870d-104">Элемент **имена внутренних доменов** определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="c870d-104">The **InternalDomains** element identifies the list of internal SMTP domains of the organization.</span></span> 
  
```XML
<InternalDomains>
   <Domain/>
</InternalDomains>
```

 <span data-ttu-id="c870d-105">**смтпдомаинлист**</span><span class="sxs-lookup"><span data-stu-id="c870d-105">**SmtpDomainList**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c870d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c870d-106">Attributes and elements</span></span>

<span data-ttu-id="c870d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c870d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c870d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c870d-108">Attributes</span></span>

<span data-ttu-id="c870d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c870d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c870d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c870d-110">Child elements</span></span>

|<span data-ttu-id="c870d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c870d-111">**Element**</span></span>|<span data-ttu-id="c870d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c870d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c870d-113">Домен</span><span class="sxs-lookup"><span data-stu-id="c870d-113">Domain</span></span>](domain.md) <br/> |<span data-ttu-id="c870d-114">Определяет один домен SMTP.</span><span class="sxs-lookup"><span data-stu-id="c870d-114">Identifies a single SMTP domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c870d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c870d-115">Parent elements</span></span>

|<span data-ttu-id="c870d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c870d-116">**Element**</span></span>|<span data-ttu-id="c870d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c870d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c870d-118">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="c870d-118">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="c870d-119">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c870d-119">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="c870d-120">протектионрулесконфигуратион</span><span class="sxs-lookup"><span data-stu-id="c870d-120">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="c870d-121">Содержит сведения о конфигурации службы для службы правил защиты.</span><span class="sxs-lookup"><span data-stu-id="c870d-121">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c870d-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c870d-122">Text value</span></span>

<span data-ttu-id="c870d-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c870d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c870d-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="c870d-124">Remarks</span></span>

<span data-ttu-id="c870d-125">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="c870d-125">This element is required.</span></span> 
  
<span data-ttu-id="c870d-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c870d-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c870d-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c870d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c870d-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c870d-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c870d-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c870d-129">Schema Name</span></span>  <br/> |<span data-ttu-id="c870d-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c870d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="c870d-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c870d-131">Validation File</span></span>  <br/> |<span data-ttu-id="c870d-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c870d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c870d-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c870d-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="c870d-134">False</span><span class="sxs-lookup"><span data-stu-id="c870d-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c870d-135">См. также</span><span class="sxs-lookup"><span data-stu-id="c870d-135">See also</span></span>



- [<span data-ttu-id="c870d-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c870d-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

