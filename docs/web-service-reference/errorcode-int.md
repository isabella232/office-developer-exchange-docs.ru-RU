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
ms.openlocfilehash: 24170a56e5fa23c3811fcbd27f0240e6ba3c87b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460668"
---
# <a name="errorcode-int"></a><span data-ttu-id="f3cce-103">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="f3cce-103">ErrorCode (int)</span></span>

<span data-ttu-id="f3cce-104">Элемент **ErrorCode** указывает код ошибки при неудачном поиске, выполненном для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f3cce-104">The **ErrorCode** element specifies the error code of a failed search performed against a mailbox.</span></span> 
  
```XML
<ErrorCode></ErrorCode>
```

 <span data-ttu-id="f3cce-105">**int**</span><span class="sxs-lookup"><span data-stu-id="f3cce-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3cce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3cce-106">Attributes and elements</span></span>

<span data-ttu-id="f3cce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3cce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3cce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3cce-108">Attributes</span></span>

<span data-ttu-id="f3cce-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3cce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3cce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3cce-110">Child elements</span></span>

<span data-ttu-id="f3cce-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3cce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3cce-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3cce-112">Parent elements</span></span>

|<span data-ttu-id="f3cce-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3cce-113">**Element**</span></span>|<span data-ttu-id="f3cce-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3cce-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3cce-115">фаиледмаилбокс</span><span class="sxs-lookup"><span data-stu-id="f3cce-115">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="f3cce-116">Указывает состояние удержания почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f3cce-116">Specifies the hold status of the mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f3cce-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f3cce-117">Text value</span></span>

<span data-ttu-id="f3cce-118">Текстовое значение элемента **ErrorCode** — это код ошибки, возвращенный для неудачного поиска, выполненного для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f3cce-118">The text value of the **ErrorCode** element is the error code returned for a failed search performed against a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f3cce-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3cce-119">Remarks</span></span>

<span data-ttu-id="f3cce-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3cce-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3cce-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3cce-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3cce-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3cce-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3cce-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3cce-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3cce-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3cce-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f3cce-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="f3cce-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="f3cce-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3cce-126">Validation File</span></span>  <br/> |<span data-ttu-id="f3cce-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f3cce-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3cce-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3cce-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f3cce-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f3cce-129">See also</span></span>



- [<span data-ttu-id="f3cce-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f3cce-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

