---
title: DiscoverySearchConfigurations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: Элемент DiscoverySearchConfigurations указывает массив элементов DiscoverySearchConfiguration.
ms.openlocfilehash: a95bb35b88114e8e72e22de424679993fd4eef2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762154"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="b059d-103">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="b059d-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="b059d-104">Элемент **DiscoverySearchConfigurations** указывает массив элементов **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="b059d-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="b059d-105">**ArrayOfDiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="b059d-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b059d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b059d-106">Attributes and elements</span></span>

<span data-ttu-id="b059d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b059d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b059d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b059d-108">Attributes</span></span>

<span data-ttu-id="b059d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b059d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b059d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b059d-110">Child elements</span></span>

|<span data-ttu-id="b059d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b059d-111">**Element**</span></span>|<span data-ttu-id="b059d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b059d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b059d-113">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="b059d-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="b059d-114">Задает конфигурацию для поиска обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="b059d-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b059d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b059d-115">Parent elements</span></span>

|<span data-ttu-id="b059d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b059d-116">**Element**</span></span>|<span data-ttu-id="b059d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b059d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b059d-118">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b059d-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="b059d-119">Задает сообщение ответа на запрос **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="b059d-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b059d-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="b059d-120">Remarks</span></span>

<span data-ttu-id="b059d-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b059d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b059d-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b059d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b059d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b059d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b059d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b059d-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b059d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b059d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b059d-126">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="b059d-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="b059d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b059d-127">Validation File</span></span>  <br/> |<span data-ttu-id="b059d-128">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b059d-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b059d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b059d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b059d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="b059d-130">See also</span></span>

- [<span data-ttu-id="b059d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b059d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
