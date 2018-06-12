---
title: DiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: Элемент DiscoverySearchConfiguration указывает конфигурацию для поиска обнаружения электронных данных.
ms.openlocfilehash: 11bf90d8fe73bb0b308deb7ae51f1443488f87e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762145"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="2b888-103">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b888-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="2b888-104">Элемент **DiscoverySearchConfiguration** указывает конфигурацию для поиска обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="2b888-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="2b888-105">**DiscoverySearchConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="2b888-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b888-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2b888-106">Attributes and elements</span></span>

<span data-ttu-id="2b888-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2b888-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b888-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b888-108">Attributes</span></span>

<span data-ttu-id="2b888-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b888-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b888-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b888-110">Child elements</span></span>

|<span data-ttu-id="2b888-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b888-111">**Element**</span></span>|<span data-ttu-id="2b888-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b888-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b888-113">SearchId</span><span class="sxs-lookup"><span data-stu-id="2b888-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="2b888-114">Задает идентификатор для поиска.</span><span class="sxs-lookup"><span data-stu-id="2b888-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="2b888-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="2b888-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="2b888-116">Указывает имя запроса поиска eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="2b888-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="2b888-117">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="2b888-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="2b888-118">Содержит список почтовых ящиков, возвращаемый запросом **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="2b888-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b888-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2b888-119">Parent elements</span></span>

|<span data-ttu-id="2b888-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b888-120">**Element**</span></span>|<span data-ttu-id="2b888-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b888-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b888-122">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="2b888-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="2b888-123">Указывает массив элементов **DiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="2b888-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b888-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="2b888-124">Remarks</span></span>

<span data-ttu-id="2b888-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2b888-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b888-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b888-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b888-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2b888-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b888-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2b888-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2b888-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2b888-129">Schema Name</span></span>  <br/> |<span data-ttu-id="2b888-130">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="2b888-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="2b888-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2b888-131">Validation File</span></span>  <br/> |<span data-ttu-id="2b888-132">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2b888-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2b888-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2b888-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2b888-134">См. также</span><span class="sxs-lookup"><span data-stu-id="2b888-134">See also</span></span>

- [<span data-ttu-id="2b888-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2b888-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

