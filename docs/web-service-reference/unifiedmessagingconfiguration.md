---
title: UnifiedMessagingConfiguration
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
description: Элемент UnifiedMessagingConfiguration содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.
ms.openlocfilehash: 3ad8f66ecdf21062c00c2a6ac6f65fac875da38c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840269"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="0f296-103">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f296-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="0f296-104">Элемент **UnifiedMessagingConfiguration** содержит сведения о конфигурации службы для службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="0f296-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="0f296-105">**UnifiedMessageServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="0f296-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f296-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0f296-106">Attributes and elements</span></span>

<span data-ttu-id="0f296-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0f296-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f296-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0f296-108">Attributes</span></span>

<span data-ttu-id="0f296-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f296-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f296-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0f296-110">Child elements</span></span>

|<span data-ttu-id="0f296-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f296-111">**Element**</span></span>|<span data-ttu-id="0f296-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f296-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f296-113">UmEnabled</span><span class="sxs-lookup"><span data-stu-id="0f296-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="0f296-114">Указывает, включена ли единой системы обмена сообщениями для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="0f296-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="0f296-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f296-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0f296-116">PlayOnPhoneDialString (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="0f296-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="0f296-117">Определяет строку телефонным воспроизвести на телефоне.</span><span class="sxs-lookup"><span data-stu-id="0f296-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="0f296-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f296-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="0f296-119">PlayOnPhoneEnabled</span><span class="sxs-lookup"><span data-stu-id="0f296-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="0f296-120">Указывает, включена ли функция воспроизвести на телефоне.</span><span class="sxs-lookup"><span data-stu-id="0f296-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="0f296-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f296-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f296-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0f296-122">Parent elements</span></span>

|<span data-ttu-id="0f296-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0f296-123">**Element**</span></span>|<span data-ttu-id="0f296-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0f296-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f296-125">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="0f296-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="0f296-126">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="0f296-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f296-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0f296-127">Text value</span></span>

<span data-ttu-id="0f296-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="0f296-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f296-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="0f296-129">Remarks</span></span>

<span data-ttu-id="0f296-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f296-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f296-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0f296-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f296-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0f296-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0f296-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0f296-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0f296-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0f296-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0f296-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0f296-135">Validation File</span></span>  <br/> |<span data-ttu-id="0f296-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0f296-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0f296-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0f296-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f296-138">False</span><span class="sxs-lookup"><span data-stu-id="0f296-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f296-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0f296-139">See also</span></span>



- [<span data-ttu-id="0f296-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0f296-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

