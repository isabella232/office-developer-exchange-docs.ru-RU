---
title: дисковерисеарчконфигуратионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f04b14c9-384c-4016-b113-52a49e15e73b
description: Элемент Дисковерисеарчконфигуратионс указывает массив элементов Дисковерисеарчконфигуратион.
ms.openlocfilehash: 6af4c8198f2ad73f8b39f9718e11b88aa8075c39
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461382"
---
# <a name="discoverysearchconfigurations"></a><span data-ttu-id="39955-103">дисковерисеарчконфигуратионс</span><span class="sxs-lookup"><span data-stu-id="39955-103">DiscoverySearchConfigurations</span></span>

<span data-ttu-id="39955-104">Элемент **дисковерисеарчконфигуратионс** указывает массив элементов **дисковерисеарчконфигуратион** .</span><span class="sxs-lookup"><span data-stu-id="39955-104">The **DiscoverySearchConfigurations** element specifies an array of **DiscoverySearchConfiguration** elements.</span></span> 
  
```XML
<DiscoverySearchConfigurations>
    <DiscoverySearchConfiguration></DiscoverySearchConfiguration>
</DiscoverySearchConfigurations>
```

 <span data-ttu-id="39955-105">**аррайофдисковерисеарчконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="39955-105">**ArrayOfDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39955-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="39955-106">Attributes and elements</span></span>

<span data-ttu-id="39955-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="39955-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39955-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="39955-108">Attributes</span></span>

<span data-ttu-id="39955-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39955-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39955-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="39955-110">Child elements</span></span>

|<span data-ttu-id="39955-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39955-111">**Element**</span></span>|<span data-ttu-id="39955-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39955-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39955-113">дисковерисеарчконфигуратион</span><span class="sxs-lookup"><span data-stu-id="39955-113">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md) <br/> |<span data-ttu-id="39955-114">Задает конфигурацию для поиска обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="39955-114">Specifies the configuration for eDiscovery search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39955-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="39955-115">Parent elements</span></span>

|<span data-ttu-id="39955-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39955-116">**Element**</span></span>|<span data-ttu-id="39955-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39955-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39955-118">жетдисковерисеарчконфигуратионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="39955-118">GetDiscoverySearchConfigurationResponseMessage</span></span>](getdiscoverysearchconfigurationresponsemessage.md) <br/> |<span data-ttu-id="39955-119">Задает ответное сообщение для запроса **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="39955-119">Specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="39955-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="39955-120">Remarks</span></span>

<span data-ttu-id="39955-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="39955-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="39955-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="39955-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39955-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="39955-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39955-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="39955-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39955-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="39955-125">Schema Name</span></span>  <br/> |<span data-ttu-id="39955-126">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="39955-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="39955-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="39955-127">Validation File</span></span>  <br/> |<span data-ttu-id="39955-128">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="39955-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39955-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="39955-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="39955-130">См. также</span><span class="sxs-lookup"><span data-stu-id="39955-130">See also</span></span>

- [<span data-ttu-id="39955-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39955-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

