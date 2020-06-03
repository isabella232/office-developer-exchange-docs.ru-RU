---
title: експандграупмембершип
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8989e96b-8fa1-4858-93b2-2cbdb30b9ca9
description: Элемент Експандграупмембершип указывает, следует ли расширять членство в группе, возвращенной из запроса GetSearchableMailboxes.
ms.openlocfilehash: 8a94aa3da165ecc13282127e75c8d166f3972ead
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456908"
---
# <a name="expandgroupmembership"></a><span data-ttu-id="713f9-103">експандграупмембершип</span><span class="sxs-lookup"><span data-stu-id="713f9-103">ExpandGroupMembership</span></span>

<span data-ttu-id="713f9-104">Элемент **експандграупмембершип** указывает, следует ли расширять членство в группе, возвращенной из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="713f9-104">The **ExpandGroupMembership** element indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span> 
  
```XML
<ExpandGroupMembership>true | false</ExpandGroupMembership>
```

 <span data-ttu-id="713f9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="713f9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="713f9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="713f9-106">Attributes and elements</span></span>

<span data-ttu-id="713f9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="713f9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="713f9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="713f9-108">Attributes</span></span>

<span data-ttu-id="713f9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="713f9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="713f9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="713f9-110">Child elements</span></span>

<span data-ttu-id="713f9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="713f9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="713f9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="713f9-112">Parent elements</span></span>

<span data-ttu-id="713f9-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)  |  [GetSearchableMailboxes](getsearchablemailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="713f9-113">[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md) | [GetSearchableMailboxes](getsearchablemailboxes.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="713f9-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="713f9-114">Text value</span></span>

<span data-ttu-id="713f9-115">Текстовое значение **true** для элемента **експандграупелемент** указывает на то, что членство в группе развернуто.</span><span class="sxs-lookup"><span data-stu-id="713f9-115">A text value of **true** for the **ExpandGroupElement** element indicates that group membership is expanded.</span></span> <span data-ttu-id="713f9-116">Значение **false** указывает, что членство в группе не разворачивается для отображения членов группы.</span><span class="sxs-lookup"><span data-stu-id="713f9-116">A value of **false** indicates that the group membership is not expanded to show the members of the group.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="713f9-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="713f9-117">Remarks</span></span>

<span data-ttu-id="713f9-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="713f9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="713f9-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="713f9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="713f9-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="713f9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="713f9-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="713f9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="713f9-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="713f9-122">Schema name</span></span>  <br/> |<span data-ttu-id="713f9-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="713f9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="713f9-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="713f9-124">Validation file</span></span>  <br/> |<span data-ttu-id="713f9-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="713f9-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="713f9-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="713f9-126">Can be empty</span></span>  <br/> |<span data-ttu-id="713f9-127">false</span><span class="sxs-lookup"><span data-stu-id="713f9-127">false</span></span>  <br/> |
   

