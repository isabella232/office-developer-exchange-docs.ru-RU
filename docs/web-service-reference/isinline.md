---
title: IsInline
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInline
api_type:
- schema
ms.assetid: 5e7712c8-372a-4a16-be64-360c5ff3961a
description: Элемент IsInline указывает ли вложение встроенным в элемент.
ms.openlocfilehash: f2f9093777a3914de067ef63827de6cf354fc12d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834042"
---
# <a name="isinline"></a><span data-ttu-id="92350-103">IsInline</span><span class="sxs-lookup"><span data-stu-id="92350-103">IsInline</span></span>

<span data-ttu-id="92350-104">Элемент **IsInline** указывает ли вложение встроенным в элемент.</span><span class="sxs-lookup"><span data-stu-id="92350-104">The **IsInline** element represents whether the attachment appears inline within an item.</span></span> 
  
```xml
<IsInline>true or false</IsInline>
```

 <span data-ttu-id="92350-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="92350-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92350-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="92350-106">Attributes and elements</span></span>

<span data-ttu-id="92350-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="92350-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92350-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="92350-108">Attributes</span></span>

<span data-ttu-id="92350-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="92350-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="92350-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="92350-110">Child elements</span></span>

<span data-ttu-id="92350-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="92350-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="92350-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="92350-112">Parent elements</span></span>

|<span data-ttu-id="92350-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="92350-113">**Element**</span></span>|<span data-ttu-id="92350-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="92350-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92350-115">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="92350-115">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="92350-116">Представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="92350-116">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="92350-117">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="92350-117">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="92350-118">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="92350-118">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92350-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="92350-119">Text value</span></span>

<span data-ttu-id="92350-120">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="92350-120">This element can be either **true** or **false**.</span></span> <span data-ttu-id="92350-121">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="92350-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="92350-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="92350-122">Remarks</span></span>

<span data-ttu-id="92350-123">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="92350-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92350-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="92350-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92350-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="92350-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="92350-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="92350-126">Schema Name</span></span>  <br/> |<span data-ttu-id="92350-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="92350-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="92350-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="92350-128">Validation File</span></span>  <br/> |<span data-ttu-id="92350-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="92350-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="92350-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="92350-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="92350-131">False</span><span class="sxs-lookup"><span data-stu-id="92350-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92350-132">См. также</span><span class="sxs-lookup"><span data-stu-id="92350-132">See also</span></span>



- [<span data-ttu-id="92350-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="92350-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

