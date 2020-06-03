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
ms.openlocfilehash: 8dfe5c745896d02217cbf91375d355954a4e22eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464702"
---
# <a name="applicationroles"></a><span data-ttu-id="64079-103">аппликатионролес</span><span class="sxs-lookup"><span data-stu-id="64079-103">ApplicationRoles</span></span>

<span data-ttu-id="64079-104">Элемент **аппликатионролес** указывает роли приложения, используемые вызывающим партнерским приложением для текущего вызова.</span><span class="sxs-lookup"><span data-stu-id="64079-104">The **ApplicationRoles** element specifies the application roles that the calling partner application uses for the current call.</span></span> 
  
```XML
<ApplicationRoles>
    <Role></Role>
</ApplicationRoles>
```

 <span data-ttu-id="64079-105">**нонемптяррайофролетипе**</span><span class="sxs-lookup"><span data-stu-id="64079-105">**NonEmptyArrayOfRoleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64079-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64079-106">Attributes and elements</span></span>

<span data-ttu-id="64079-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="64079-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64079-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64079-108">Attributes</span></span>

<span data-ttu-id="64079-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64079-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64079-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64079-110">Child elements</span></span>

|<span data-ttu-id="64079-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64079-111">**Element**</span></span>|<span data-ttu-id="64079-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64079-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64079-113">Role</span><span class="sxs-lookup"><span data-stu-id="64079-113">Role</span></span>](role.md) <br/> |<span data-ttu-id="64079-114">Указывает строку, представляющую роль управления.</span><span class="sxs-lookup"><span data-stu-id="64079-114">Specifies a string that represents a management role.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64079-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64079-115">Parent elements</span></span>

|<span data-ttu-id="64079-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64079-116">**Element**</span></span>|<span data-ttu-id="64079-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64079-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64079-118">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="64079-118">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="64079-119">Указывает роль управления.</span><span class="sxs-lookup"><span data-stu-id="64079-119">Specifies the management role.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64079-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="64079-120">Remarks</span></span>

<span data-ttu-id="64079-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="64079-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64079-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="64079-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64079-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64079-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64079-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64079-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64079-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64079-125">Schema Name</span></span>  <br/> |<span data-ttu-id="64079-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="64079-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="64079-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64079-127">Validation File</span></span>  <br/> |<span data-ttu-id="64079-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="64079-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="64079-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64079-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="64079-130">См. также</span><span class="sxs-lookup"><span data-stu-id="64079-130">See also</span></span>

- [<span data-ttu-id="64079-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="64079-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

