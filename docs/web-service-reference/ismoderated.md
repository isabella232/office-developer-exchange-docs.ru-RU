---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: Элемент IsModerated указывает, является ли управляемым почтовый ящик получателя.
ms.openlocfilehash: 8db234f9706bb8187978a76f745323749d7a640a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834055"
---
# <a name="ismoderated"></a><span data-ttu-id="ed282-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="ed282-103">IsModerated</span></span>

<span data-ttu-id="ed282-104">Элемент **IsModerated** указывает, является ли управляемым почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="ed282-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="ed282-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ed282-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed282-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ed282-106">Attributes and elements</span></span>

<span data-ttu-id="ed282-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ed282-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed282-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ed282-108">Attributes</span></span>

<span data-ttu-id="ed282-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ed282-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed282-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ed282-110">Child elements</span></span>

<span data-ttu-id="ed282-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ed282-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed282-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ed282-112">Parent elements</span></span>

|<span data-ttu-id="ed282-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ed282-113">**Element**</span></span>|<span data-ttu-id="ed282-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ed282-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed282-115">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="ed282-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ed282-116">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="ed282-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed282-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ed282-117">Text value</span></span>

<span data-ttu-id="ed282-118">Текстовое значение для этого элемента — это **значение true,** Если проходят контроль почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="ed282-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="ed282-119">Значение равно **false** , если почтовый ящик получателя не является управляемым.</span><span class="sxs-lookup"><span data-stu-id="ed282-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ed282-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="ed282-120">Remarks</span></span>

<span data-ttu-id="ed282-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed282-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed282-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ed282-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed282-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ed282-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed282-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ed282-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ed282-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ed282-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed282-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ed282-126">Validation File</span></span>  <br/> |<span data-ttu-id="ed282-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ed282-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed282-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ed282-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed282-129">False</span><span class="sxs-lookup"><span data-stu-id="ed282-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed282-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ed282-130">See also</span></span>



- [<span data-ttu-id="ed282-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ed282-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

