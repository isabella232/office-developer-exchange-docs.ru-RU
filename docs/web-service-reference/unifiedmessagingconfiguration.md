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
ms.openlocfilehash: 3ad8f66ecdf21062c00c2a6ac6f65fac875da38c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840269"
---
# <a name="unifiedmessagingconfiguration"></a><span data-ttu-id="ece5d-103">унифиедмессагингконфигуратион</span><span class="sxs-lookup"><span data-stu-id="ece5d-103">UnifiedMessagingConfiguration</span></span>

<span data-ttu-id="ece5d-104">Элемент **унифиедмессагингконфигуратион** содержит сведения о конфигурации службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="ece5d-104">The **UnifiedMessagingConfiguration** element contains service configuration information for the Unified Messaging service.</span></span> 
  
```XML
<UnifiedMessagingConfiguration>
   <UmEnabled/>
   <PlayOnPhoneDialString/>
   <PlayOnPhoneEnabled/>
</UnifiedMessagingConfiguration>
```

 <span data-ttu-id="ece5d-105">**унифиедмессажесервицеконфигуратион**</span><span class="sxs-lookup"><span data-stu-id="ece5d-105">**UnifiedMessageServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ece5d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ece5d-106">Attributes and elements</span></span>

<span data-ttu-id="ece5d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ece5d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ece5d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ece5d-108">Attributes</span></span>

<span data-ttu-id="ece5d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ece5d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ece5d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ece5d-110">Child elements</span></span>

|<span data-ttu-id="ece5d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ece5d-111">**Element**</span></span>|<span data-ttu-id="ece5d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ece5d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ece5d-113">уменаблед</span><span class="sxs-lookup"><span data-stu-id="ece5d-113">UmEnabled</span></span>](umenabled.md) <br/> |<span data-ttu-id="ece5d-114">Указывает, включена ли единая система обмена сообщениями для учетной записи.</span><span class="sxs-lookup"><span data-stu-id="ece5d-114">Indicates whether Unified Messaging is enabled for an account.</span></span> <span data-ttu-id="ece5d-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece5d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ece5d-116">Плайонфонедиалстринг (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="ece5d-116">PlayOnPhoneDialString (Exchange Web Services)</span></span>](playonphonedialstring-exchange-web-services.md) <br/> |<span data-ttu-id="ece5d-117">Определяет строку набора номера для проигрывания телефона.</span><span class="sxs-lookup"><span data-stu-id="ece5d-117">Identifies the Play-on-Phone dial string.</span></span> <span data-ttu-id="ece5d-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece5d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="ece5d-119">плайонфонинаблед</span><span class="sxs-lookup"><span data-stu-id="ece5d-119">PlayOnPhoneEnabled</span></span>](playonphoneenabled.md) <br/> |<span data-ttu-id="ece5d-120">Указывает, включена ли функция проигрывания на телефоне.</span><span class="sxs-lookup"><span data-stu-id="ece5d-120">Indicates whether the Play-on-Phone feature is enabled.</span></span> <span data-ttu-id="ece5d-121">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="ece5d-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ece5d-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ece5d-122">Parent elements</span></span>

|<span data-ttu-id="ece5d-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ece5d-123">**Element**</span></span>|<span data-ttu-id="ece5d-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ece5d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ece5d-125">сервицеконфигуратионреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="ece5d-125">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="ece5d-126">Содержит параметры конфигурации службы.</span><span class="sxs-lookup"><span data-stu-id="ece5d-126">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ece5d-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ece5d-127">Text value</span></span>

<span data-ttu-id="ece5d-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="ece5d-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ece5d-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="ece5d-129">Remarks</span></span>

<span data-ttu-id="ece5d-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ece5d-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ece5d-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ece5d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ece5d-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ece5d-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ece5d-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ece5d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ece5d-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ece5d-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ece5d-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ece5d-135">Validation File</span></span>  <br/> |<span data-ttu-id="ece5d-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ece5d-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ece5d-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ece5d-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ece5d-138">False</span><span class="sxs-lookup"><span data-stu-id="ece5d-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ece5d-139">См. также</span><span class="sxs-lookup"><span data-stu-id="ece5d-139">See also</span></span>



- [<span data-ttu-id="ece5d-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ece5d-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

