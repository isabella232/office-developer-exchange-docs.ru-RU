---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: Элемент InstallApp указывает запрос на установку приложения.
ms.openlocfilehash: d9b7412865c003b89eccbdd92aa6ff9968048191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833949"
---
# <a name="installapp"></a><span data-ttu-id="e497d-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="e497d-103">InstallApp</span></span>

<span data-ttu-id="e497d-104">Элемент **InstallApp** указывает запрос на установку приложения.</span><span class="sxs-lookup"><span data-stu-id="e497d-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="e497d-105">**InstallAppType**</span><span class="sxs-lookup"><span data-stu-id="e497d-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e497d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e497d-106">Attributes and elements</span></span>

<span data-ttu-id="e497d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e497d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e497d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e497d-108">Attributes</span></span>

<span data-ttu-id="e497d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e497d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e497d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e497d-110">Child elements</span></span>

|<span data-ttu-id="e497d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e497d-111">**Element**</span></span>|<span data-ttu-id="e497d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e497d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e497d-113">Манифест</span><span class="sxs-lookup"><span data-stu-id="e497d-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="e497d-114">Содержит файл манифеста приложения в кодировке base64.</span><span class="sxs-lookup"><span data-stu-id="e497d-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e497d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e497d-115">Parent elements</span></span>

<span data-ttu-id="e497d-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="e497d-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e497d-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="e497d-117">Remarks</span></span>

<span data-ttu-id="e497d-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e497d-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e497d-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e497d-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e497d-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e497d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e497d-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e497d-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e497d-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e497d-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e497d-123">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="e497d-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="e497d-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e497d-124">Validation File</span></span>  <br/> |<span data-ttu-id="e497d-125">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e497d-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e497d-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e497d-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e497d-127">См. также</span><span class="sxs-lookup"><span data-stu-id="e497d-127">See also</span></span>



- [<span data-ttu-id="e497d-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e497d-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

