---
title: аппликатионролес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00003b9b-f8f1-4452-a0af-157f789f8892
description: Элемент Аппликатионролес указывает роли приложения, используемые вызывающим партнерским приложением для текущего вызова.
ms.openlocfilehash: ff32b693dae573416263bcb7c0fbb552a933b8d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761392"
---
# <a name="applicationroles"></a><span data-ttu-id="bdc93-103">аппликатионролес</span><span class="sxs-lookup"><span data-stu-id="bdc93-103">ApplicationRoles</span></span>

<span data-ttu-id="bdc93-104">Элемент **аппликатионролес** указывает роли приложения, используемые вызывающим партнерским приложением для текущего вызова.</span><span class="sxs-lookup"><span data-stu-id="bdc93-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="bdc93-105">**нонемптяррайофролетипе**</span><span class="sxs-lookup"><span data-stu-id="bdc93-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdc93-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bdc93-106">Attributes and elements</span></span>

<span data-ttu-id="bdc93-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bdc93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdc93-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bdc93-108">Attributes</span></span>

<span data-ttu-id="bdc93-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bdc93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdc93-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bdc93-110">Child elements</span></span>

|<span data-ttu-id="bdc93-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bdc93-111">**Element**</span></span>|<span data-ttu-id="bdc93-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bdc93-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdc93-113">Роль</span><span class="sxs-lookup"><span data-stu-id="bdc93-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="bdc93-114">Указывает строку, представляющую роль управления.</span><span class="sxs-lookup"><span data-stu-id="bdc93-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bdc93-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bdc93-115">Parent elements</span></span>

|<span data-ttu-id="bdc93-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bdc93-116">**Element**</span></span>|<span data-ttu-id="bdc93-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bdc93-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdc93-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="bdc93-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="bdc93-119">Указывает роль управления.</span><span class="sxs-lookup"><span data-stu-id="bdc93-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bdc93-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="bdc93-120">Remarks</span></span>

<span data-ttu-id="bdc93-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bdc93-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bdc93-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bdc93-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdc93-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bdc93-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdc93-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bdc93-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bdc93-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bdc93-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bdc93-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="bdc93-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="bdc93-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bdc93-127">Validation File</span></span>  <br/> |<span data-ttu-id="bdc93-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bdc93-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="bdc93-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bdc93-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="bdc93-130">См. также</span><span class="sxs-lookup"><span data-stu-id="bdc93-130">See also</span></span>

- [<span data-ttu-id="bdc93-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bdc93-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

