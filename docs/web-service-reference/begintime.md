---
title: бегинтиме
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2a60c89c-9c21-4041-9593-b244ac1608ef
description: Элемент Бегинтиме указывает начало интервала времени, в течение которого запрашиваются напоминания.
ms.openlocfilehash: 4f926b8e4931c187cd4d5b97d6182d609bc15a1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463379"
---
# <a name="begintime"></a><span data-ttu-id="1c455-103">бегинтиме</span><span class="sxs-lookup"><span data-stu-id="1c455-103">BeginTime</span></span>

<span data-ttu-id="1c455-104">Элемент **бегинтиме** указывает начало интервала времени, в течение которого запрашиваются напоминания.</span><span class="sxs-lookup"><span data-stu-id="1c455-104">The **BeginTime** element specifies the beginning of the time span to query for reminders.</span></span> 
  
```XML
<BeginTime/>
```

 <span data-ttu-id="1c455-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="1c455-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1c455-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1c455-106">Attributes and elements</span></span>

<span data-ttu-id="1c455-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1c455-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1c455-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1c455-108">Attributes</span></span>

<span data-ttu-id="1c455-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1c455-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1c455-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1c455-110">Child elements</span></span>

<span data-ttu-id="1c455-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1c455-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1c455-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1c455-112">Parent elements</span></span>

[<span data-ttu-id="1c455-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="1c455-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="1c455-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1c455-114">Text value</span></span>

<span data-ttu-id="1c455-115">Текстовое значение элемента **бегинтиме** — время начала элемента, для которого предназначено напоминание.</span><span class="sxs-lookup"><span data-stu-id="1c455-115">The text value of the **BeginTime** element is the beginning time of the item the reminder is for.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1c455-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="1c455-116">Remarks</span></span>

<span data-ttu-id="1c455-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1c455-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1c455-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c455-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1c455-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1c455-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1c455-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1c455-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1c455-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1c455-121">Schema Name</span></span>  <br/> |<span data-ttu-id="1c455-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1c455-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1c455-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1c455-123">Validation File</span></span>  <br/> |<span data-ttu-id="1c455-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1c455-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1c455-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1c455-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="1c455-126">False</span><span class="sxs-lookup"><span data-stu-id="1c455-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1c455-127">См. также</span><span class="sxs-lookup"><span data-stu-id="1c455-127">See also</span></span>



[<span data-ttu-id="1c455-128">GetReminders</span><span class="sxs-lookup"><span data-stu-id="1c455-128">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="1c455-129">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1c455-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

