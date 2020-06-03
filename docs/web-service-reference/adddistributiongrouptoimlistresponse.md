---
title: адддистрибутионграуптоимлистреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70fe6730-1c9a-4550-acc4-7737ff407871
description: Элемент Адддистрибутионграуптоимлистреспонсе определяет ответ на запрос AddDistributionGroupToImList.
ms.openlocfilehash: 84a477dcf27bc215d330ab0a2870dc2850130fdc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460367"
---
# <a name="adddistributiongrouptoimlistresponse"></a><span data-ttu-id="96aff-103">адддистрибутионграуптоимлистреспонсе</span><span class="sxs-lookup"><span data-stu-id="96aff-103">AddDistributionGroupToImListResponse</span></span>

<span data-ttu-id="96aff-104">Элемент **адддистрибутионграуптоимлистреспонсе** определяет ответ на запрос **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="96aff-104">The **AddDistributionGroupToImListResponse** element defines a response to a **AddDistributionGroupToImList** request.</span></span> 
  
```XML
<AddNewImContactToGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImGroup/>
</AddNewImContactToGroupResponse>
```

 <span data-ttu-id="96aff-105">**адддистрибутионграуптоимлистреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="96aff-105">**AddDistributionGroupToImListResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="96aff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="96aff-106">Attributes and elements</span></span>

<span data-ttu-id="96aff-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="96aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="96aff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="96aff-108">Attributes</span></span>

<span data-ttu-id="96aff-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="96aff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="96aff-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="96aff-110">Child elements</span></span>

<span data-ttu-id="96aff-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Группа](imgroup.md)</span><span class="sxs-lookup"><span data-stu-id="96aff-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="96aff-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="96aff-112">Parent elements</span></span>

<span data-ttu-id="96aff-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="96aff-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="96aff-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="96aff-114">Remarks</span></span>

<span data-ttu-id="96aff-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="96aff-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="96aff-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="96aff-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="96aff-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="96aff-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="96aff-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="96aff-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="96aff-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="96aff-119">Schema name</span></span>  <br/> |<span data-ttu-id="96aff-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="96aff-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="96aff-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="96aff-121">Validation file</span></span>  <br/> |<span data-ttu-id="96aff-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="96aff-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="96aff-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="96aff-123">Can be empty</span></span>  <br/> |<span data-ttu-id="96aff-124">false</span><span class="sxs-lookup"><span data-stu-id="96aff-124">false</span></span>  <br/> |
   

