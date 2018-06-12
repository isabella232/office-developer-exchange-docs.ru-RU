---
title: HasPicture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasPicture
api_type:
- schema
ms.assetid: 922a43fe-01bd-49f2-9261-e00e4699b8da
description: Элемент HasPicture указывает, имеет ли элемент контактов вложенный файл, который представляет на изображение контакта.
ms.openlocfilehash: 8f6890ec2bcc9a961f69331fb20f5cad8a59bf38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833806"
---
# <a name="haspicture"></a><span data-ttu-id="42484-103">HasPicture</span><span class="sxs-lookup"><span data-stu-id="42484-103">HasPicture</span></span>

<span data-ttu-id="42484-104">Элемент **HasPicture** указывает, имеет ли элемент контактов вложенный файл, который представляет на изображение контакта.</span><span class="sxs-lookup"><span data-stu-id="42484-104">The **HasPicture** element indicates whether the contact item has a file attachment that represents the contact's picture.</span></span> 
  
[<span data-ttu-id="42484-105">Контакт</span><span class="sxs-lookup"><span data-stu-id="42484-105">Contact</span></span>](contact.md)
  
[<span data-ttu-id="42484-106">HasPicture</span><span class="sxs-lookup"><span data-stu-id="42484-106">HasPicture</span></span>](haspicture.md)
  
```xml
<HasPicture>true or false</HasPicture>
```

 <span data-ttu-id="42484-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="42484-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42484-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="42484-108">Attributes and elements</span></span>

<span data-ttu-id="42484-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="42484-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42484-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="42484-110">Attributes</span></span>

<span data-ttu-id="42484-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="42484-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42484-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="42484-112">Child elements</span></span>

<span data-ttu-id="42484-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="42484-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42484-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="42484-114">Parent elements</span></span>

|<span data-ttu-id="42484-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="42484-115">**Element**</span></span>|<span data-ttu-id="42484-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="42484-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42484-117">Контакт</span><span class="sxs-lookup"><span data-stu-id="42484-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="42484-118">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="42484-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="42484-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="42484-119">Text value</span></span>

<span data-ttu-id="42484-120">Текстовое значение элемента **HasPicture** может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="42484-120">The text value of the **HasPicture** element can be either **true** or **false**.</span></span> <span data-ttu-id="42484-121">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="42484-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="42484-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="42484-122">Remarks</span></span>

<span data-ttu-id="42484-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="42484-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42484-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="42484-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42484-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="42484-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42484-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="42484-126">Schema Name</span></span>  <br/> |<span data-ttu-id="42484-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="42484-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="42484-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="42484-128">Validation File</span></span>  <br/> |<span data-ttu-id="42484-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42484-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42484-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="42484-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="42484-131">False</span><span class="sxs-lookup"><span data-stu-id="42484-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42484-132">См. также</span><span class="sxs-lookup"><span data-stu-id="42484-132">See also</span></span>



- [<span data-ttu-id="42484-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="42484-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

