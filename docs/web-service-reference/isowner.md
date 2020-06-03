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
ms.openlocfilehash: 2dd085aba34052d95efd1e72edca7be4aba71155
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466523"
---
# <a name="isowner"></a><span data-ttu-id="190cc-103">Владелец</span><span class="sxs-lookup"><span data-stu-id="190cc-103">IsOwner</span></span>

<span data-ttu-id="190cc-104">Элемент **owner** указывает, является ли указанный пользователь электронной почты владельцем.</span><span class="sxs-lookup"><span data-stu-id="190cc-104">The **IsOwner** element specifies whether the specified email user is the owner.</span></span> 
  
```XML
<IsOwner>true | false</IsOwner>
```

 <span data-ttu-id="190cc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="190cc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="190cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="190cc-106">Attributes and elements</span></span>

<span data-ttu-id="190cc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="190cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="190cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="190cc-108">Attributes</span></span>

<span data-ttu-id="190cc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="190cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="190cc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="190cc-110">Child elements</span></span>

<span data-ttu-id="190cc-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="190cc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="190cc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="190cc-112">Parent elements</span></span>

|<span data-ttu-id="190cc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="190cc-113">**Element**</span></span>|<span data-ttu-id="190cc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="190cc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="190cc-115">ригхтсманажементлиценседата</span><span class="sxs-lookup"><span data-stu-id="190cc-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="190cc-116">Указывает сведения о лицензии на управление правами.</span><span class="sxs-lookup"><span data-stu-id="190cc-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="190cc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="190cc-117">Text value</span></span>

<span data-ttu-id="190cc-118">Текстовое значение **true** для элемента **owner** указывает на то, что пользователь является владельцем прав, выданных для элемента.</span><span class="sxs-lookup"><span data-stu-id="190cc-118">A text value of **true** for the **IsOwner** element indicates that the user is the owner of rights issued on an item.</span></span> <span data-ttu-id="190cc-119">Значение **false** указывает, что пользователь не является владельцем прав, выданных для элемента.</span><span class="sxs-lookup"><span data-stu-id="190cc-119">A value of **false** indicates that the user is not the owner of rights issued on an item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="190cc-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="190cc-120">Remarks</span></span>

<span data-ttu-id="190cc-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="190cc-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="190cc-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="190cc-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="190cc-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="190cc-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="190cc-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="190cc-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="190cc-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="190cc-125">Schema Name</span></span>  <br/> |<span data-ttu-id="190cc-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="190cc-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="190cc-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="190cc-127">Validation File</span></span>  <br/> |<span data-ttu-id="190cc-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="190cc-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="190cc-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="190cc-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="190cc-130">См. также</span><span class="sxs-lookup"><span data-stu-id="190cc-130">See also</span></span>



- [<span data-ttu-id="190cc-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="190cc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

