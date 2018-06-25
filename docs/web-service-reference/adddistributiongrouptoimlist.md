---
title: AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: adbffbfc-e436-4620-acfc-5dfd41a88cb8
description: Элемент AddDistributionGroupToImList определяет запрос на добавление в список рассылки в список мгновенное сообщение.
ms.openlocfilehash: b63daeb8b1d60123215bfcdec307f2f948d2ec39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761338"
---
# <a name="adddistributiongrouptoimlist"></a><span data-ttu-id="56ba2-103">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="56ba2-103">AddDistributionGroupToImList</span></span>

<span data-ttu-id="56ba2-104">Элемент **AddDistributionGroupToImList** определяет запрос на добавление в список рассылки в список мгновенное сообщение.</span><span class="sxs-lookup"><span data-stu-id="56ba2-104">The **AddDistributionGroupToImList** element defines a request to add a distribution list to an instant message list.</span></span> 
  
```XML
<AddDistributionGroupToImList>
   <SmtpAddress/>
   <DisplayName/>
</AddDistributionGroupToImList>
```

 <span data-ttu-id="56ba2-105">**AddDistributionGroupToImListType**</span><span class="sxs-lookup"><span data-stu-id="56ba2-105">**AddDistributionGroupToImListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56ba2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="56ba2-106">Attributes and elements</span></span>

<span data-ttu-id="56ba2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="56ba2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56ba2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="56ba2-108">Attributes</span></span>

<span data-ttu-id="56ba2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="56ba2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56ba2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="56ba2-110">Child elements</span></span>

<span data-ttu-id="56ba2-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="56ba2-111">[SmtpAddress](smtpaddress.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56ba2-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="56ba2-112">Parent elements</span></span>

<span data-ttu-id="56ba2-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="56ba2-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56ba2-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="56ba2-114">Remarks</span></span>

<span data-ttu-id="56ba2-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="56ba2-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="56ba2-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="56ba2-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56ba2-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="56ba2-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56ba2-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="56ba2-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56ba2-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="56ba2-119">Schema name</span></span>  <br/> |<span data-ttu-id="56ba2-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="56ba2-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="56ba2-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="56ba2-121">Validation file</span></span>  <br/> |<span data-ttu-id="56ba2-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="56ba2-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56ba2-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="56ba2-123">Can be empty</span></span>  <br/> |<span data-ttu-id="56ba2-124">Нет</span><span class="sxs-lookup"><span data-stu-id="56ba2-124">false</span></span>  <br/> |
   

