---
title: Владелец
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: Элемент Owner указывает, является ли указанный пользователь электронной почты владельцем.
ms.openlocfilehash: aac3c2a599093282542025468d73c55ec4569e29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834080"
---
# <a name="isowner"></a><span data-ttu-id="ce661-103">Владелец</span><span class="sxs-lookup"><span data-stu-id="ce661-103">IsOwner</span></span>

<span data-ttu-id="ce661-104">Элемент **owner** указывает, является ли указанный пользователь электронной почты владельцем.</span><span class="sxs-lookup"><span data-stu-id="ce661-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="ce661-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ce661-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce661-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ce661-106">Attributes and elements</span></span>

<span data-ttu-id="ce661-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ce661-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce661-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ce661-108">Attributes</span></span>

<span data-ttu-id="ce661-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce661-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce661-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ce661-110">Child elements</span></span>

<span data-ttu-id="ce661-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce661-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ce661-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ce661-112">Parent elements</span></span>

|<span data-ttu-id="ce661-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce661-113">**Element**</span></span>|<span data-ttu-id="ce661-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce661-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce661-115">ригхтсманажементлиценседата</span><span class="sxs-lookup"><span data-stu-id="ce661-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="ce661-116">Указывает сведения о лицензии на управление правами.</span><span class="sxs-lookup"><span data-stu-id="ce661-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ce661-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ce661-117">Text value</span></span>

<span data-ttu-id="ce661-118">Текстовое значение **true** для элемента **owner** указывает на то, что пользователь является владельцем прав, выданных для элемента.</span><span class="sxs-lookup"><span data-stu-id="ce661-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="ce661-119">Значение **false** указывает, что пользователь не является владельцем прав, выданных для элемента.</span><span class="sxs-lookup"><span data-stu-id="ce661-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ce661-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="ce661-120">Remarks</span></span>

<span data-ttu-id="ce661-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ce661-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ce661-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce661-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ce661-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ce661-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce661-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ce661-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ce661-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ce661-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ce661-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="ce661-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="ce661-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ce661-127">Validation File</span></span>  <br/> |<span data-ttu-id="ce661-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ce661-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ce661-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ce661-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ce661-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ce661-130">See also</span></span>



- [<span data-ttu-id="ce661-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ce661-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

