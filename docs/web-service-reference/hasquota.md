---
title: HasQuota
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: Элемент HasQuota указывает, будет ли управляемой папки квоту.
ms.openlocfilehash: 26f14ee7c9d4de267733bca11f7884d1d391b3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833807"
---
# <a name="hasquota"></a><span data-ttu-id="6d080-103">HasQuota</span><span class="sxs-lookup"><span data-stu-id="6d080-103">HasQuota</span></span>

<span data-ttu-id="6d080-104">Элемент **HasQuota** указывает, будет ли управляемой папки квоту.</span><span class="sxs-lookup"><span data-stu-id="6d080-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="6d080-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6d080-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6d080-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6d080-106">Attributes and elements</span></span>

<span data-ttu-id="6d080-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6d080-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d080-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6d080-108">Attributes</span></span>

<span data-ttu-id="6d080-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6d080-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d080-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6d080-110">Child elements</span></span>

<span data-ttu-id="6d080-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6d080-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6d080-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6d080-112">Parent elements</span></span>

|<span data-ttu-id="6d080-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d080-113">**Element**</span></span>|<span data-ttu-id="6d080-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d080-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d080-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="6d080-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="6d080-116">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="6d080-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6d080-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6d080-117">Text value</span></span>

<span data-ttu-id="6d080-118">Текстовое значение представляет значение типа Boolean.</span><span class="sxs-lookup"><span data-stu-id="6d080-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="6d080-119">Значение **true** означает, что папка квот; значение **false** указывает, что папка не имеет квоты.</span><span class="sxs-lookup"><span data-stu-id="6d080-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6d080-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="6d080-120">Remarks</span></span>

<span data-ttu-id="6d080-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6d080-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d080-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6d080-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d080-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6d080-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d080-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6d080-124">Schema name</span></span>  <br/> |<span data-ttu-id="6d080-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6d080-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d080-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6d080-126">Validation file</span></span>  <br/> |<span data-ttu-id="6d080-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d080-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d080-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6d080-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6d080-129">False</span><span class="sxs-lookup"><span data-stu-id="6d080-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d080-130">См. также</span><span class="sxs-lookup"><span data-stu-id="6d080-130">See also</span></span>



- [<span data-ttu-id="6d080-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6d080-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

