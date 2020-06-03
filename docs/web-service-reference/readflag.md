---
title: реадфлаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9d91aa89-9f9f-4877-846d-aaf48bbeec7c
description: Элемент Реадфлаг указывает состояние чтения, которое необходимо задать для элементов в папке.
ms.openlocfilehash: 1d3b9f3fe199ed2e63bdb632135120a5f89f4d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529898"
---
# <a name="readflag"></a><span data-ttu-id="8304c-103">реадфлаг</span><span class="sxs-lookup"><span data-stu-id="8304c-103">ReadFlag</span></span>

<span data-ttu-id="8304c-104">Элемент **реадфлаг** указывает состояние чтения, которое необходимо задать для элементов в папке.</span><span class="sxs-lookup"><span data-stu-id="8304c-104">The **ReadFlag** element indicates the read state to set on items in a folder.</span></span> 
  
```XML
<ReadFlag>true | false</ReadFlag>
```

 <span data-ttu-id="8304c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8304c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8304c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8304c-106">Attributes and elements</span></span>

<span data-ttu-id="8304c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8304c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8304c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8304c-108">Attributes</span></span>

<span data-ttu-id="8304c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8304c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8304c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8304c-110">Child elements</span></span>

<span data-ttu-id="8304c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8304c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8304c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8304c-112">Parent elements</span></span>

[<span data-ttu-id="8304c-113">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="8304c-113">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
  
## <a name="text-value"></a><span data-ttu-id="8304c-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8304c-114">Text value</span></span>

<span data-ttu-id="8304c-115">Текстовое значение **true** для элемента **реадфлаг** указывает на то, что элементы в папке помечаются как прочтенные.</span><span class="sxs-lookup"><span data-stu-id="8304c-115">A text value of **true** for the **ReadFlag** element indicates that the items in the folder will be marked as read.</span></span> <span data-ttu-id="8304c-116">Значение **false** указывает на то, что элементы в папке помечаются как непрочтенные.</span><span class="sxs-lookup"><span data-stu-id="8304c-116">A value of **false** indicates that the items in the folder will be marked as unread.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8304c-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="8304c-117">Remarks</span></span>

<span data-ttu-id="8304c-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8304c-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8304c-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8304c-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8304c-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8304c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8304c-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8304c-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8304c-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8304c-122">Schema name</span></span>  <br/> |<span data-ttu-id="8304c-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8304c-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8304c-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8304c-124">Validation file</span></span>  <br/> |<span data-ttu-id="8304c-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8304c-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8304c-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8304c-126">Can be empty</span></span>  <br/> ||
   

