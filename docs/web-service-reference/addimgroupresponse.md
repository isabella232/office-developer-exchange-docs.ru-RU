---
title: аддимграупреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2fca9474-f5f8-44e8-975d-145fc7696edf
description: Аддимграупреспонсе определяет ответ на запрос AddImGroup.
ms.openlocfilehash: 1fc7a2cd8c86a6ac7ce1d23d4b62fc6b2ade9d70
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761345"
---
# <a name="addimgroupresponse"></a><span data-ttu-id="3b9f2-103">аддимграупреспонсе</span><span class="sxs-lookup"><span data-stu-id="3b9f2-103">AddImGroupResponse</span></span>

<span data-ttu-id="3b9f2-104">**Аддимграупреспонсе** определяет ответ на запрос **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="3b9f2-104">The **AddImGroupResponse** defines a response to an **AddImGroup** request.</span></span> 
  
```XML
<AddImGroupResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ImGroup/>
</AddImGroupResponse>
```

 <span data-ttu-id="3b9f2-105">**аддимконтакттограупреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="3b9f2-105">**AddImContactToGroupResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b9f2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b9f2-106">Attributes and elements</span></span>

<span data-ttu-id="3b9f2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3b9f2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b9f2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b9f2-108">Attributes</span></span>

<span data-ttu-id="3b9f2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b9f2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b9f2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b9f2-110">Child elements</span></span>

<span data-ttu-id="3b9f2-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [ImGroup](imgroup.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл |  | </span><span class="sxs-lookup"><span data-stu-id="3b9f2-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ImGroup](imgroup.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b9f2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b9f2-112">Parent elements</span></span>

<span data-ttu-id="3b9f2-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b9f2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b9f2-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b9f2-114">Remarks</span></span>

<span data-ttu-id="3b9f2-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3b9f2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3b9f2-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3b9f2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b9f2-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b9f2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b9f2-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b9f2-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b9f2-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b9f2-119">Schema name</span></span>  <br/> |<span data-ttu-id="3b9f2-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3b9f2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b9f2-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b9f2-121">Validation file</span></span>  <br/> |<span data-ttu-id="3b9f2-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3b9f2-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b9f2-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b9f2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3b9f2-124">false</span><span class="sxs-lookup"><span data-stu-id="3b9f2-124">false</span></span>  <br/> |
   

