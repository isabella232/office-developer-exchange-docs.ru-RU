---
title: SuppressReadReceipts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: Следует подавлять SuppressReadReceipts, элемент показывает, является ли уведомления о прочтении.
ms.openlocfilehash: 794252da6b3e6b6e6f36181c1811a2a001bfaf53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840118"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="f0094-103">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="f0094-103">SuppressReadReceipts</span></span>

<span data-ttu-id="f0094-104">Элемент **SuppressReadReceipts** указывает ли чтение квитанций необходимо было отменено.</span><span class="sxs-lookup"><span data-stu-id="f0094-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="f0094-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f0094-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0094-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0094-106">Attributes and elements</span></span>

<span data-ttu-id="f0094-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f0094-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0094-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0094-108">Attributes</span></span>

<span data-ttu-id="f0094-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0094-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0094-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0094-110">Child elements</span></span>

<span data-ttu-id="f0094-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f0094-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0094-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0094-112">Parent elements</span></span>

<span data-ttu-id="f0094-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="f0094-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f0094-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f0094-114">Text value</span></span>

<span data-ttu-id="f0094-115">Текстовое значение **true** для элемента **SuppressReadReciepts** указывает, что чтения, подавляются поступлений.</span><span class="sxs-lookup"><span data-stu-id="f0094-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="f0094-116">Значение **false** указывает, что чтения, которые будут отправляться уведомления для отправителя.</span><span class="sxs-lookup"><span data-stu-id="f0094-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f0094-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="f0094-117">Remarks</span></span>

<span data-ttu-id="f0094-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f0094-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f0094-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f0094-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0094-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0094-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0094-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0094-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0094-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0094-122">Schema name</span></span>  <br/> |<span data-ttu-id="f0094-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f0094-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0094-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0094-124">Validation file</span></span>  <br/> |<span data-ttu-id="f0094-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0094-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0094-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0094-126">Can be empty</span></span>  <br/> ||
   

