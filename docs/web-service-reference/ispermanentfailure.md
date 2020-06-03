---
title: исперманентфаилуре
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: Элемент Исперманентфаилуре указывает, была ли предыдущая попытка индексировать элемент завершилась неудачно.
ms.openlocfilehash: 48a13eebfa16c538c1b10d92f080d51f1b318d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460395"
---
# <a name="ispermanentfailure"></a><span data-ttu-id="c81f9-103">исперманентфаилуре</span><span class="sxs-lookup"><span data-stu-id="c81f9-103">IsPermanentFailure</span></span>

<span data-ttu-id="c81f9-104">Элемент **исперманентфаилуре** указывает, была ли предыдущая попытка индексировать элемент завершилась неудачно.</span><span class="sxs-lookup"><span data-stu-id="c81f9-104">The **IsPermanentFailure** element indicates whether a previous attempt to index the item was unsuccessful.</span></span> 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 <span data-ttu-id="c81f9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c81f9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c81f9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c81f9-106">Attributes and elements</span></span>

<span data-ttu-id="c81f9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c81f9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c81f9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c81f9-108">Attributes</span></span>

<span data-ttu-id="c81f9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c81f9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c81f9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c81f9-110">Child elements</span></span>

<span data-ttu-id="c81f9-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c81f9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c81f9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c81f9-112">Parent elements</span></span>

[<span data-ttu-id="c81f9-113">нониндексаблеитемдетаил</span><span class="sxs-lookup"><span data-stu-id="c81f9-113">NonIndexableItemDetail</span></span>](nonindexableitemdetail.md)
  
## <a name="text-value"></a><span data-ttu-id="c81f9-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c81f9-114">Text value</span></span>

<span data-ttu-id="c81f9-115">Текстовое значение **true** для элемента **исперманентфаилуре** указывает на то, что предыдущая попытка индексирования элемента почтового ящика выполнена неудачно.</span><span class="sxs-lookup"><span data-stu-id="c81f9-115">A text value of **true** for the **IsPermanentFailure** element indicates that a previous attempt to index the mailbox item was unsuccessful.</span></span> <span data-ttu-id="c81f9-116">Значение **false** указывает, что предыдущая попытка индексировать элемент почтового ящика выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="c81f9-116">A value of **false** indicates that a previous attempt to index the mailbox item was successful.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c81f9-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="c81f9-117">Remarks</span></span>

<span data-ttu-id="c81f9-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c81f9-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c81f9-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c81f9-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c81f9-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c81f9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c81f9-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c81f9-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c81f9-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c81f9-122">Schema name</span></span>  <br/> |<span data-ttu-id="c81f9-123">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c81f9-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="c81f9-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c81f9-124">Validation file</span></span>  <br/> |<span data-ttu-id="c81f9-125">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c81f9-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c81f9-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c81f9-126">Can be empty</span></span>  <br/> |<span data-ttu-id="c81f9-127">false</span><span class="sxs-lookup"><span data-stu-id="c81f9-127">false</span></span>  <br/> |
   

