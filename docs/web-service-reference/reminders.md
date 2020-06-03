---
title: Reminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 19294300-ab84-4784-8aa7-3395a08de640
description: Элемент памятки указывает напоминания, возвращаемые в ответе на запрос с помощью распомниок.
ms.openlocfilehash: 1ddf1c10872dcce103919dbed3d1c5e04cdfca74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458497"
---
# <a name="reminders"></a><span data-ttu-id="74fa9-103">Reminders</span><span class="sxs-lookup"><span data-stu-id="74fa9-103">Reminders</span></span>

<span data-ttu-id="74fa9-104">Элемент **памятки** указывает напоминания, возвращаемые в ответе на запрос с помощью **распомниок** .</span><span class="sxs-lookup"><span data-stu-id="74fa9-104">The **Reminders** element specifies the reminders returned in the response to a **GetReminders** request.</span></span> 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 <span data-ttu-id="74fa9-105">**аррайофреминдерстипе**</span><span class="sxs-lookup"><span data-stu-id="74fa9-105">**ArrayOfRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74fa9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="74fa9-106">Attributes and elements</span></span>

<span data-ttu-id="74fa9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="74fa9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74fa9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="74fa9-108">Attributes</span></span>

<span data-ttu-id="74fa9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="74fa9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74fa9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="74fa9-110">Child elements</span></span>

[<span data-ttu-id="74fa9-111">Reminder</span><span class="sxs-lookup"><span data-stu-id="74fa9-111">Reminder</span></span>](reminder.md)
  
### <a name="parent-elements"></a><span data-ttu-id="74fa9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="74fa9-112">Parent elements</span></span>

[<span data-ttu-id="74fa9-113">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="74fa9-113">GetRemindersResponse</span></span>](getremindersresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="74fa9-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="74fa9-114">Remarks</span></span>

<span data-ttu-id="74fa9-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="74fa9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="74fa9-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="74fa9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74fa9-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="74fa9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74fa9-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="74fa9-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74fa9-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="74fa9-119">Schema Name</span></span>  <br/> |<span data-ttu-id="74fa9-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="74fa9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74fa9-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="74fa9-121">Validation File</span></span>  <br/> |<span data-ttu-id="74fa9-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="74fa9-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74fa9-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="74fa9-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="74fa9-124">False</span><span class="sxs-lookup"><span data-stu-id="74fa9-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74fa9-125">См. также</span><span class="sxs-lookup"><span data-stu-id="74fa9-125">See also</span></span>



[<span data-ttu-id="74fa9-126">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="74fa9-126">GetRemindersResponse</span></span>](getremindersresponse.md)


- [<span data-ttu-id="74fa9-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="74fa9-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

