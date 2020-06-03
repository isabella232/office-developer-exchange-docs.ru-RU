---
title: дисковерисеарчконфигуратион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 085384f9-dca4-4534-82e2-dd782471d0da
description: Элемент Дисковерисеарчконфигуратион указывает конфигурацию для поиска обнаружения электронных данных.
ms.openlocfilehash: 8819d951f35ccc215bdf0128d2a16b60bbf20f2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529058"
---
# <a name="discoverysearchconfiguration"></a><span data-ttu-id="1a7a5-103">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="1a7a5-103">DiscoverySearchConfiguration</span></span>

<span data-ttu-id="1a7a5-104">Элемент **дисковерисеарчконфигуратион** указывает конфигурацию для поиска обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-104">The **DiscoverySearchConfiguration** element specifies the configuration for eDiscovery search.</span></span> 
  
```XML
<DiscoverySearchConfiguration>
    <SearchId></SearchId>
    <SearchQuery></SearchQuery>
    <SearchableMailboxes></SearchableMailboxes>
</DiscoverySearchConfiguration>
```

 <span data-ttu-id="1a7a5-105">**дисковерисеарчконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="1a7a5-105">**DiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a7a5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a7a5-106">Attributes and elements</span></span>

<span data-ttu-id="1a7a5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a7a5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a7a5-108">Attributes</span></span>

<span data-ttu-id="1a7a5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a7a5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a7a5-110">Child elements</span></span>

|<span data-ttu-id="1a7a5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a7a5-111">**Element**</span></span>|<span data-ttu-id="1a7a5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a7a5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a7a5-113">сеарчид</span><span class="sxs-lookup"><span data-stu-id="1a7a5-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="1a7a5-114">Задает идентификатор поиска.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="1a7a5-115">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="1a7a5-115">SearchQuery</span></span>](searchquery.md) <br/> |<span data-ttu-id="1a7a5-116">Задает имя поискового запроса обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-116">Specifies the name of an eDiscovery search query.</span></span>  <br/> |
|[<span data-ttu-id="1a7a5-117">сеарчаблемаилбоксес</span><span class="sxs-lookup"><span data-stu-id="1a7a5-117">SearchableMailboxes</span></span>](searchablemailboxes.md) <br/> |<span data-ttu-id="1a7a5-118">Содержит список почтовых ящиков, возвращенных из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="1a7a5-118">Contains a list of the mailboxes returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a7a5-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a7a5-119">Parent elements</span></span>

|<span data-ttu-id="1a7a5-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a7a5-120">**Element**</span></span>|<span data-ttu-id="1a7a5-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a7a5-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a7a5-122">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="1a7a5-122">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md) <br/> |<span data-ttu-id="1a7a5-123">Указывает массив элементов **дисковерисеарчконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="1a7a5-123">Specifies an array of **DiscoverySearchConfiguration** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1a7a5-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="1a7a5-124">Remarks</span></span>

<span data-ttu-id="1a7a5-125">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1a7a5-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a7a5-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a7a5-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a7a5-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a7a5-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a7a5-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a7a5-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a7a5-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1a7a5-130">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="1a7a5-130">Message schema</span></span>  <br/> |
|<span data-ttu-id="1a7a5-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a7a5-131">Validation File</span></span>  <br/> |<span data-ttu-id="1a7a5-132">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1a7a5-132">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a7a5-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a7a5-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1a7a5-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1a7a5-134">See also</span></span>

- [<span data-ttu-id="1a7a5-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1a7a5-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

