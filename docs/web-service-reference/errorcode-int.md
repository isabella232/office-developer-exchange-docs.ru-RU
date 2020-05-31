---
title: ErrorCode (int)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65537d96-edf9-41ee-9ad5-91ffe37e2269
description: Элемент ErrorCode указывает код ошибки при неудачном поиске, выполненном для почтового ящика.
ms.openlocfilehash: ed8a7771376f921303ea093f4be727c4146faa76
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762377"
---
# <a name="errorcode-int"></a><span data-ttu-id="a4119-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="a4119-103">ErrorCode (int)</span></span>

<span data-ttu-id="a4119-104">Элемент **ErrorCode** указывает код ошибки при неудачном поиске, выполненном для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a4119-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="a4119-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a4119-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4119-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a4119-106">Attributes and elements</span></span>

<span data-ttu-id="a4119-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a4119-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4119-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a4119-108">Attributes</span></span>

<span data-ttu-id="a4119-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4119-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4119-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a4119-110">Child elements</span></span>

<span data-ttu-id="a4119-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4119-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4119-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a4119-112">Parent elements</span></span>

|<span data-ttu-id="a4119-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a4119-113">**Element**</span></span>|<span data-ttu-id="a4119-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a4119-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4119-115">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="a4119-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="a4119-116">Указывает состояние удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a4119-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4119-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a4119-117">Text value</span></span>

<span data-ttu-id="a4119-118">Текстовое значение элемента **ErrorCode** — это код ошибки, возвращенный для неудачного поиска, выполненного для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a4119-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4119-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="a4119-119">Remarks</span></span>

<span data-ttu-id="a4119-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a4119-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a4119-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a4119-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4119-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a4119-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4119-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a4119-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4119-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a4119-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a4119-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="a4119-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="a4119-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a4119-126">Validation File</span></span>  <br/> |<span data-ttu-id="a4119-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a4119-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4119-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a4119-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a4119-129">См. также</span><span class="sxs-lookup"><span data-stu-id="a4119-129">See also</span></span>



- [<span data-ttu-id="a4119-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a4119-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

