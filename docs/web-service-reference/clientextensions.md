---
title: ClientExtensions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0073d195-75fd-4c89-97e0-2ad6d91f99f9
description: Элемент ClientExtensions содержит массив пользователя и настройки сведений о приложениях.
ms.openlocfilehash: c2f2511154daaded09ba0e8d811baf9ce30ca138
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761688"
---
# <a name="clientextensions"></a><span data-ttu-id="e2fc8-103">ClientExtensions</span><span class="sxs-lookup"><span data-stu-id="e2fc8-103">ClientExtensions</span></span>

<span data-ttu-id="e2fc8-104">Элемент **ClientExtensions** содержит массив пользователя и настройки сведений о приложениях.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-104">The **ClientExtensions** element contains an array of user and configuration information about apps.</span></span> 
  
```XML
<ClientExtensions>
   <ClientExtension/>
</ClientExtensions>
```

 <span data-ttu-id="e2fc8-105">**ArrayOfClientExtensionsType**</span><span class="sxs-lookup"><span data-stu-id="e2fc8-105">**ArrayOfClientExtensionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2fc8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2fc8-106">Attributes and elements</span></span>

<span data-ttu-id="e2fc8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2fc8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2fc8-108">Attributes</span></span>

<span data-ttu-id="e2fc8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2fc8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2fc8-110">Child elements</span></span>

|<span data-ttu-id="e2fc8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2fc8-111">**Element**</span></span>|<span data-ttu-id="e2fc8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2fc8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2fc8-113">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="e2fc8-113">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="e2fc8-114">Содержит пользователей и конфигурации сведения о приложении.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-114">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2fc8-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2fc8-115">Parent elements</span></span>

|<span data-ttu-id="e2fc8-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2fc8-116">**Element**</span></span>|<span data-ttu-id="e2fc8-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2fc8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2fc8-118">GetClientExtensionResponse</span><span class="sxs-lookup"><span data-stu-id="e2fc8-118">GetClientExtensionResponse</span></span>](getclientextensionresponse.md) <br/> |<span data-ttu-id="e2fc8-119">Представляет ответа для получения сведений о приложении конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-119">Represents a response to get configuration information about an app.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2fc8-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="e2fc8-120">Remarks</span></span>

<span data-ttu-id="e2fc8-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2fc8-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2fc8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2fc8-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2fc8-123">Element information</span></span>

||
|:-----|
|<span data-ttu-id="e2fc8-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2fc8-124">Namespace</span></span>  <br/> |
|<span data-ttu-id="e2fc8-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2fc8-125">Schema Name</span></span>  <br/> |
|<span data-ttu-id="e2fc8-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2fc8-126">Validation File</span></span>  <br/> |
|<span data-ttu-id="e2fc8-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2fc8-127">Can be Empty</span></span>  <br/> |
   

