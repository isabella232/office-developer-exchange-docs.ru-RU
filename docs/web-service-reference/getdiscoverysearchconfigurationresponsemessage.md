---
title: жетдисковерисеарчконфигуратионреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b84a4c6-cb0a-4bca-85b2-fec32227930b
description: Элемент Жетдисковерисеарчконфигуратионреспонсемессаже указывает ответное сообщение для запроса GetDiscoverySearchConfiguration.
ms.openlocfilehash: 23d1c5b7a61a9161d7383ec8b38cd0ebbebfc8cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460976"
---
# <a name="getdiscoverysearchconfigurationresponsemessage"></a><span data-ttu-id="d1e57-103">жетдисковерисеарчконфигуратионреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="d1e57-103">GetDiscoverySearchConfigurationResponseMessage</span></span>

<span data-ttu-id="d1e57-104">Элемент **жетдисковерисеарчконфигуратионреспонсемессаже** указывает ответное сообщение для запроса **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d1e57-104">The **GetDiscoverySearchConfigurationResponseMessage** element specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponseMessage>
```

 <span data-ttu-id="d1e57-105">**жетдисковерисеарчконфигуратионреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="d1e57-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1e57-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d1e57-106">Attributes and elements</span></span>

<span data-ttu-id="d1e57-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d1e57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1e57-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d1e57-108">Attributes</span></span>

<span data-ttu-id="d1e57-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d1e57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1e57-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d1e57-110">Child elements</span></span>

<span data-ttu-id="d1e57-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Дисковерисеарчконфигуратионс](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="d1e57-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1e57-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d1e57-112">Parent elements</span></span>

[<span data-ttu-id="d1e57-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="d1e57-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="d1e57-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="d1e57-114">Remarks</span></span>

<span data-ttu-id="d1e57-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d1e57-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d1e57-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1e57-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1e57-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d1e57-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1e57-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d1e57-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1e57-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d1e57-119">Schema name</span></span>  <br/> |<span data-ttu-id="d1e57-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d1e57-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1e57-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d1e57-121">Validation file</span></span>  <br/> |<span data-ttu-id="d1e57-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d1e57-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1e57-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d1e57-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d1e57-124">false</span><span class="sxs-lookup"><span data-stu-id="d1e57-124">false</span></span>  <br/> |
   

