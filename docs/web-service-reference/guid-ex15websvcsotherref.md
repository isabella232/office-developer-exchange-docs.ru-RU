---
title: Guid
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 49dcf69f-bf8d-4be6-a24c-03bbd13f4fe5
description: Элемент GUID указывает глобальный уникальный идентификатор почтового ящика.
ms.openlocfilehash: 4db66b5ae2c67f64f75c69a3d77cfa2b587775be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530777"
---
# <a name="guid"></a><span data-ttu-id="4531b-103">Guid</span><span class="sxs-lookup"><span data-stu-id="4531b-103">Guid</span></span>

<span data-ttu-id="4531b-104">Элемент **GUID** указывает глобальный уникальный идентификатор почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="4531b-104">The **Guid** element specifies the globally unique identifier of the mailbox.</span></span> 
  
```XML
<Guid></Guid>
```

 <span data-ttu-id="4531b-105">**гуидтипе**</span><span class="sxs-lookup"><span data-stu-id="4531b-105">**GuidType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4531b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4531b-106">Attributes and elements</span></span>

<span data-ttu-id="4531b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4531b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4531b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4531b-108">Attributes</span></span>

<span data-ttu-id="4531b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4531b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4531b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4531b-110">Child elements</span></span>

<span data-ttu-id="4531b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4531b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4531b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4531b-112">Parent elements</span></span>

|<span data-ttu-id="4531b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4531b-113">**Element**</span></span>|<span data-ttu-id="4531b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4531b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4531b-115">сеарчаблемаилбокс</span><span class="sxs-lookup"><span data-stu-id="4531b-115">SearchableMailbox</span></span>](searchablemailbox.md) <br/> |<span data-ttu-id="4531b-116">Указывает почтовый ящик, возвращенный из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="4531b-116">Specifies a mailbox returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4531b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4531b-117">Text value</span></span>

<span data-ttu-id="4531b-118">Текстовое значение элемента **GUID** — это значение GUID, которое уникально определяет почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="4531b-118">The text value of the **Guid** element is a GUID value that uniquely identifies a mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4531b-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="4531b-119">Remarks</span></span>

<span data-ttu-id="4531b-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4531b-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4531b-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4531b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4531b-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4531b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4531b-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4531b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4531b-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4531b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4531b-125">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4531b-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="4531b-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4531b-126">Validation File</span></span>  <br/> |<span data-ttu-id="4531b-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4531b-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4531b-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4531b-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4531b-129">См. также</span><span class="sxs-lookup"><span data-stu-id="4531b-129">See also</span></span>



- [<span data-ttu-id="4531b-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4531b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

