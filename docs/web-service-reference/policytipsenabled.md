---
title: PolicyTipsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 16409652-21e4-4bd3-9373-67e1882236b4
description: Элемент PolicyTipsEnabled указывает, включены ли подсказки политики.
ms.openlocfilehash: 683131a5cefd6757faf582324f312b01fd9ddb33
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834838"
---
# <a name="policytipsenabled"></a><span data-ttu-id="2b3ce-103">PolicyTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="2b3ce-103">PolicyTipsEnabled</span></span>

<span data-ttu-id="2b3ce-104">Элемент **PolicyTipsEnabled** указывает, включены ли подсказки политики.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-104">The **PolicyTipsEnabled** element indicates whether policy tips are enabled.</span></span> 
  
```XML
<PolicyTipsEnabled> true | false </PolicyTipsEnabled>
```

 <span data-ttu-id="2b3ce-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2b3ce-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b3ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2b3ce-106">Attributes and elements</span></span>

<span data-ttu-id="2b3ce-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b3ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b3ce-108">Attributes</span></span>

<span data-ttu-id="2b3ce-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b3ce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b3ce-110">Child elements</span></span>

<span data-ttu-id="2b3ce-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b3ce-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2b3ce-112">Parent elements</span></span>

[<span data-ttu-id="2b3ce-113">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="2b3ce-113">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md)
  
## <a name="text-value"></a><span data-ttu-id="2b3ce-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2b3ce-114">Text value</span></span>

<span data-ttu-id="2b3ce-115">Текстовое значение **true** для элемента **PolicyTipsEnabled** указывает, что советы по политикам разрешены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-115">A text value of **true** for the **PolicyTipsEnabled** element indicates that policy tips are enabled for a mailbox.</span></span> <span data-ttu-id="2b3ce-116">Значение **false** указывает подсказок политики не включены для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-116">A value of **false** indicates that policy tips are not enabled for a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2b3ce-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="2b3ce-117">Remarks</span></span>

<span data-ttu-id="2b3ce-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b3ce-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2b3ce-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b3ce-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2b3ce-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b3ce-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2b3ce-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b3ce-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2b3ce-122">Schema name</span></span>  <br/> |<span data-ttu-id="2b3ce-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2b3ce-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b3ce-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2b3ce-124">Validation file</span></span>  <br/> |<span data-ttu-id="2b3ce-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b3ce-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b3ce-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2b3ce-126">Can be empty</span></span>  <br/> ||
   

