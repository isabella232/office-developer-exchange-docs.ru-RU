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
ms.openlocfilehash: 955fc568dc919d591076271382a8c9bbd1d146ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835071"
---
# <a name="reminders"></a><span data-ttu-id="6b3b6-103">Reminders</span><span class="sxs-lookup"><span data-stu-id="6b3b6-103">Reminders</span></span>

<span data-ttu-id="6b3b6-104">Элемент **памятки** указывает напоминания, возвращаемые в ответе на запрос с помощью **распомниок** .</span><span class="sxs-lookup"><span data-stu-id="6b3b6-104">The **Reminders** element specifies the reminders returned in the response to a **GetReminders** request.</span></span> 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 <span data-ttu-id="6b3b6-105">**аррайофреминдерстипе**</span><span class="sxs-lookup"><span data-stu-id="6b3b6-105">**ArrayOfRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b3b6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b3b6-106">Attributes and elements</span></span>

<span data-ttu-id="6b3b6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6b3b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b3b6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b3b6-108">Attributes</span></span>

<span data-ttu-id="6b3b6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b3b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b3b6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b3b6-110">Child elements</span></span>

[<span data-ttu-id="6b3b6-111">Reminder</span><span class="sxs-lookup"><span data-stu-id="6b3b6-111">Reminder</span></span>](reminder.md)
  
### <a name="parent-elements"></a><span data-ttu-id="6b3b6-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b3b6-112">Parent elements</span></span>

[<span data-ttu-id="6b3b6-113">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b3b6-113">GetRemindersResponse</span></span>](getremindersresponse.md)
  
## <a name="remarks"></a><span data-ttu-id="6b3b6-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="6b3b6-114">Remarks</span></span>

<span data-ttu-id="6b3b6-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b3b6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b3b6-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b3b6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b3b6-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b3b6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b3b6-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b3b6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b3b6-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b3b6-119">Schema Name</span></span>  <br/> |<span data-ttu-id="6b3b6-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6b3b6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b3b6-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b3b6-121">Validation File</span></span>  <br/> |<span data-ttu-id="6b3b6-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6b3b6-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b3b6-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b3b6-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b3b6-124">False</span><span class="sxs-lookup"><span data-stu-id="6b3b6-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b3b6-125">См. также</span><span class="sxs-lookup"><span data-stu-id="6b3b6-125">See also</span></span>



[<span data-ttu-id="6b3b6-126">жетреминдерсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b3b6-126">GetRemindersResponse</span></span>](getremindersresponse.md)


- [<span data-ttu-id="6b3b6-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6b3b6-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

