---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: Элемент ReminderType указывает тип напоминаний для возврата.
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835077"
---
# <a name="remindertype"></a><span data-ttu-id="bbe50-103">ReminderType</span><span class="sxs-lookup"><span data-stu-id="bbe50-103">ReminderType</span></span>

<span data-ttu-id="bbe50-104">Элемент **ReminderType** указывает тип напоминаний для возврата.</span><span class="sxs-lookup"><span data-stu-id="bbe50-104">The **ReminderType** element specifies the type of reminders to return.</span></span> 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 <span data-ttu-id="bbe50-105">**string**</span><span class="sxs-lookup"><span data-stu-id="bbe50-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bbe50-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bbe50-106">Attributes and elements</span></span>

<span data-ttu-id="bbe50-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bbe50-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbe50-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bbe50-108">Attributes</span></span>

<span data-ttu-id="bbe50-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bbe50-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bbe50-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bbe50-110">Child elements</span></span>

<span data-ttu-id="bbe50-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bbe50-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bbe50-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bbe50-112">Parent elements</span></span>

[<span data-ttu-id="bbe50-113">GetReminders</span><span class="sxs-lookup"><span data-stu-id="bbe50-113">GetReminders</span></span>](getreminders.md)
  
## <a name="text-value"></a><span data-ttu-id="bbe50-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bbe50-114">Text value</span></span>

<span data-ttu-id="bbe50-115">Текстовое значение элемента **ReminderType** — тип напоминаний для возврата **всех**, **текущей**или **старой**.</span><span class="sxs-lookup"><span data-stu-id="bbe50-115">The text value of the **ReminderType** element is the type of reminders to return, either **All**, **Current**, or **Old**.</span></span> <span data-ttu-id="bbe50-116">**Все** — это рекомендуемое значение для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bbe50-116">**All** is the recommended value for this element.</span></span> <span data-ttu-id="bbe50-117">Дополнительные сведения о связи между **ReminderType** элемент и элементы [BeginTime](begintime.md) и [EndTime](endtime-remindermessagedatatype.md) можно [GetReminders операции](getreminders-operation.md).</span><span class="sxs-lookup"><span data-stu-id="bbe50-117">For more information about the relationship between the **ReminderType** element and the [BeginTime](begintime.md) and [EndTime](endtime-remindermessagedatatype.md) elements, see [GetReminders operation](getreminders-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bbe50-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="bbe50-118">Remarks</span></span>

<span data-ttu-id="bbe50-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bbe50-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bbe50-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bbe50-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbe50-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bbe50-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbe50-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bbe50-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bbe50-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bbe50-123">Schema Name</span></span>  <br/> |<span data-ttu-id="bbe50-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bbe50-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bbe50-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bbe50-125">Validation File</span></span>  <br/> |<span data-ttu-id="bbe50-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bbe50-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bbe50-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bbe50-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbe50-128">False</span><span class="sxs-lookup"><span data-stu-id="bbe50-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbe50-129">См. также</span><span class="sxs-lookup"><span data-stu-id="bbe50-129">See also</span></span>



[<span data-ttu-id="bbe50-130">GetReminders</span><span class="sxs-lookup"><span data-stu-id="bbe50-130">GetReminders</span></span>](getreminders.md)


- [<span data-ttu-id="bbe50-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bbe50-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

