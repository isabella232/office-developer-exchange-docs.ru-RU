---
title: макеитемиммутабле
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de1d2a60-aeeb-4625-8b11-23c42e1e7bae
description: Элемент Макеитемиммутабле указывает логическое значение, которое указывает, следует ли сделать элемент только для чтения.
ms.openlocfilehash: 05c6e3343b8ba892048174ad98c9d31fe8da685b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465865"
---
# <a name="makeitemimmutable"></a><span data-ttu-id="fd6da-103">макеитемиммутабле</span><span class="sxs-lookup"><span data-stu-id="fd6da-103">MakeItemImmutable</span></span>

<span data-ttu-id="fd6da-104">Элемент **макеитемиммутабле** указывает логическое значение, которое указывает, следует ли сделать элемент только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd6da-104">The **MakeItemImmutable** element specifies a Boolean value that indicates whether an item should be made read-only.</span></span> 
  
```XML
<MakeItemImmutable>true | false</MakeItemImmutable>
```

 <span data-ttu-id="fd6da-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fd6da-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fd6da-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fd6da-106">Attributes and elements</span></span>

<span data-ttu-id="fd6da-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fd6da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fd6da-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fd6da-108">Attributes</span></span>

<span data-ttu-id="fd6da-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd6da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fd6da-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fd6da-110">Child elements</span></span>

<span data-ttu-id="fd6da-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd6da-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fd6da-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fd6da-112">Parent elements</span></span>

[<span data-ttu-id="fd6da-113">упдатеитеминрековераблеитемс</span><span class="sxs-lookup"><span data-stu-id="fd6da-113">UpdateItemInRecoverableItems</span></span>](updateiteminrecoverableitems.md)
  
## <a name="text-value"></a><span data-ttu-id="fd6da-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fd6da-114">Text value</span></span>

<span data-ttu-id="fd6da-115">Текстовое значение **true** для элемента **макеитемиммутабле** указывает на то, что элемент должен быть доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="fd6da-115">A text value of **true** for the **MakeItemImmutable** element indicates that the item should be made read-only.</span></span> <span data-ttu-id="fd6da-116">Значение **false** указывает, что элемент разрешает доступ для чтения и записи.</span><span class="sxs-lookup"><span data-stu-id="fd6da-116">A value of **false** indicates that the item allows read-write access.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fd6da-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="fd6da-117">Remarks</span></span>

<span data-ttu-id="fd6da-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fd6da-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fd6da-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fd6da-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fd6da-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fd6da-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fd6da-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fd6da-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fd6da-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fd6da-122">Schema name</span></span>  <br/> |<span data-ttu-id="fd6da-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fd6da-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fd6da-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fd6da-124">Validation file</span></span>  <br/> |<span data-ttu-id="fd6da-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fd6da-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fd6da-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fd6da-126">Can be empty</span></span>  <br/> ||
   

