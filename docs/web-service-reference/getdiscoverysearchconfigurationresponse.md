---
title: жетдисковерисеарчконфигуратионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d963e6c-e94d-462b-8c44-95d55c848fb2
description: Элемент Жетдисковерисеарчконфигуратионреспонсе указывает ответ на запрос GetDiscoverySearchConfiguration.
ms.openlocfilehash: 6f4bbc05da0c2883f78b31cb46108e993b8b8fdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762752"
---
# <a name="getdiscoverysearchconfigurationresponse"></a><span data-ttu-id="3c602-103">жетдисковерисеарчконфигуратионреспонсе</span><span class="sxs-lookup"><span data-stu-id="3c602-103">GetDiscoverySearchConfigurationResponse</span></span>

<span data-ttu-id="3c602-104">Элемент **жетдисковерисеарчконфигуратионреспонсе** указывает ответ на запрос **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="3c602-104">The **GetDiscoverySearchConfigurationResponse** element specifies the response to a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponse>
```

 <span data-ttu-id="3c602-105">**жетдисковерисеарчконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="3c602-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3c602-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3c602-106">Attributes and elements</span></span>

<span data-ttu-id="3c602-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3c602-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3c602-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3c602-108">Attributes</span></span>

<span data-ttu-id="3c602-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3c602-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3c602-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3c602-110">Child elements</span></span>

<span data-ttu-id="3c602-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл дисковерисеарчконфигуратионс |  | </span><span class="sxs-lookup"><span data-stu-id="3c602-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3c602-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3c602-112">Parent elements</span></span>

[<span data-ttu-id="3c602-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="3c602-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="3c602-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="3c602-114">Remarks</span></span>

<span data-ttu-id="3c602-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3c602-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3c602-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3c602-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3c602-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3c602-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3c602-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3c602-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3c602-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3c602-119">Schema name</span></span>  <br/> |<span data-ttu-id="3c602-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3c602-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3c602-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3c602-121">Validation file</span></span>  <br/> |<span data-ttu-id="3c602-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3c602-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3c602-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3c602-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3c602-124">false</span><span class="sxs-lookup"><span data-stu-id="3c602-124">false</span></span>  <br/> |
   

