---
title: унифиедмессагингконфигуратион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnifiedMessagingConfiguration
api_type:
- schema
ms.assetid: cbdb4268-077e-44ed-8ec2-9d759c84cc6d
description: Элемент Унифиедмессагингконфигуратион содержит сведения о конфигурации службы единой системы обмена сообщениями.
ms.openlocfilehash: 3f9f4ed65721929c552615c07e2239f48ef837f3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528694"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="5655f-103">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="5655f-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="5655f-104">Элемент **унифиедмессагингконфигуратион** содержит сведения о конфигурации службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="5655f-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="5655f-105">**унифиедмессажесервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="5655f-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5655f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5655f-106">Attributes and elements</span></span>

<span data-ttu-id="5655f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5655f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5655f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5655f-108">Attributes</span></span>

<span data-ttu-id="5655f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5655f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5655f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5655f-110">Child elements</span></span>

|<span data-ttu-id="5655f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5655f-111">**Element**</span></span>|<span data-ttu-id="5655f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5655f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5655f-113">уменаблед</span><span class="sxs-lookup"><span data-stu-id="5655f-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="5655f-114">Указывает, включена ли единая система обмена сообщениями для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="5655f-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="5655f-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="5655f-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5655f-116">Плайонфонедиалстринг (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="5655f-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="5655f-117">Определяет строку набора номера для проигрывания телефона.</span><span class="sxs-lookup"><span data-stu-id="5655f-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="5655f-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="5655f-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5655f-119">плайонфонинаблед</span><span class="sxs-lookup"><span data-stu-id="5655f-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="5655f-120">Указывает, включена ли функция проигрывания на телефоне.</span><span class="sxs-lookup"><span data-stu-id="5655f-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="5655f-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="5655f-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5655f-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5655f-122">Parent elements</span></span>

|<span data-ttu-id="5655f-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5655f-123">**Element**</span></span>|<span data-ttu-id="5655f-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5655f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5655f-125">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="5655f-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="5655f-126">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="5655f-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5655f-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5655f-127">Text value</span></span>

<span data-ttu-id="5655f-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="5655f-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5655f-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="5655f-129">Remarks</span></span>

<span data-ttu-id="5655f-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5655f-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5655f-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5655f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5655f-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5655f-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5655f-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5655f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5655f-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5655f-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5655f-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5655f-135">Validation File</span></span>  <br/> |<span data-ttu-id="5655f-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5655f-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5655f-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5655f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="5655f-138">False</span><span class="sxs-lookup"><span data-stu-id="5655f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5655f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="5655f-139">See also</span></span>



- [<span data-ttu-id="5655f-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5655f-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

