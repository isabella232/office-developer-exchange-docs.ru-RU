---
title: ReadFlag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: Элемент ReadFlag указывает состояние чтения, чтобы задать для элементов в папке.
ms.openlocfilehash: f3156a51fbdd3372dd28f2065499d26a50b3d497
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834954"
---
# <a name="readflag"></a><span data-ttu-id="a2fb1-103">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="a2fb1-103">ReadFlag</span></span>

<span data-ttu-id="a2fb1-104">Элемент **ReadFlag** указывает состояние чтения, чтобы задать для элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="a2fb1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a2fb1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2fb1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2fb1-106">Attributes and elements</span></span>

<span data-ttu-id="a2fb1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2fb1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2fb1-108">Attributes</span></span>

<span data-ttu-id="a2fb1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2fb1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2fb1-110">Child elements</span></span>

<span data-ttu-id="a2fb1-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2fb1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2fb1-112">Parent elements</span></span>

[<span data-ttu-id="a2fb1-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="a2fb1-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="a2fb1-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a2fb1-114">Text value</span></span>

<span data-ttu-id="a2fb1-115">Текстовое значение **true** для элемента **ReadFlag** указывает, что элементы в папке будут помечены как чтения.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="a2fb1-116">Значение **false** указывает, что элементы в папке будут помечены как непрочитанные.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a2fb1-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="a2fb1-117">Remarks</span></span>

<span data-ttu-id="a2fb1-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a2fb1-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a2fb1-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2fb1-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2fb1-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2fb1-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2fb1-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a2fb1-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2fb1-122">Schema name</span></span>  <br/> |<span data-ttu-id="a2fb1-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a2fb1-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a2fb1-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2fb1-124">Validation file</span></span>  <br/> |<span data-ttu-id="a2fb1-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a2fb1-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a2fb1-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2fb1-126">Can be empty</span></span>  <br/> ||
   

