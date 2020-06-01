---
title: суппрессреадрецеиптс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f0805560-7a2f-455b-94d2-ec4f1e3652c3
description: Элемент Суппрессреадрецеиптс указывает, следует ли подавлять уведомления о прочтении.
ms.openlocfilehash: aa604d4907582bd73727ba664958a589a222f9cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455935"
---
# <a name="suppressreadreceipts"></a><span data-ttu-id="3afce-103">суппрессреадрецеиптс</span><span class="sxs-lookup"><span data-stu-id="3afce-103">SuppressReadReceipts</span></span>

<span data-ttu-id="3afce-104">Элемент **суппрессреадрецеиптс** указывает, следует ли подавлять уведомления о прочтении.</span><span class="sxs-lookup"><span data-stu-id="3afce-104">The **SuppressReadReceipts** element indicates whether read receipts should be suppressed.</span></span> 
  
```XML
<SuppressReadReceipts>true | false</SuppressReadReceipts>
```

 <span data-ttu-id="3afce-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3afce-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3afce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3afce-106">Attributes and elements</span></span>

<span data-ttu-id="3afce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3afce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3afce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3afce-108">Attributes</span></span>

<span data-ttu-id="3afce-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3afce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3afce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3afce-110">Child elements</span></span>

<span data-ttu-id="3afce-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3afce-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3afce-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3afce-112">Parent elements</span></span>

<span data-ttu-id="3afce-113">[Конверсатионактион](conversationaction.md)  |  [MarkAllItemsAsRead](markallitemsasread.md)</span><span class="sxs-lookup"><span data-stu-id="3afce-113">[ConversationAction](conversationaction.md) | [MarkAllItemsAsRead](markallitemsasread.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3afce-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3afce-114">Text value</span></span>

<span data-ttu-id="3afce-115">Текстовое значение **true** для элемента **суппрессреадреЦиептс** указывает, что уведомления о прочтении подавляются.</span><span class="sxs-lookup"><span data-stu-id="3afce-115">A text value of **true** for the **SuppressReadReciepts** element indicates that read receipts are suppressed.</span></span> <span data-ttu-id="3afce-116">Значение **false** указывает, что уведомления о прочтении отправляются отправителю.</span><span class="sxs-lookup"><span data-stu-id="3afce-116">A value of **false** indicates that read receipts will be sent to the sender.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3afce-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="3afce-117">Remarks</span></span>

<span data-ttu-id="3afce-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3afce-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3afce-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3afce-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3afce-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3afce-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3afce-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3afce-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3afce-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3afce-122">Schema name</span></span>  <br/> |<span data-ttu-id="3afce-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3afce-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3afce-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3afce-124">Validation file</span></span>  <br/> |<span data-ttu-id="3afce-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3afce-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3afce-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3afce-126">Can be empty</span></span>  <br/> ||
   

