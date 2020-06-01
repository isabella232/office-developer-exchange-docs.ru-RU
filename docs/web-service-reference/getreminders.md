---
title: GetReminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 943c3d5d-7d29-4d70-932c-8a4fe44a0037
description: Элемент "пропоминать" указывает запрос на получение напоминаний.
ms.openlocfilehash: 8b869730f39876b838fbcbef3c39661238ed203c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458301"
---
# <a name="getreminders"></a><span data-ttu-id="3a06a-103">GetReminders</span><span class="sxs-lookup"><span data-stu-id="3a06a-103">GetReminders</span></span>

<span data-ttu-id="3a06a-104">Элемент " **Пропоминать** " указывает запрос на получение напоминаний.</span><span class="sxs-lookup"><span data-stu-id="3a06a-104">The **GetReminders** element specifies a request to get reminders.</span></span> 
  
```XML
<GetReminders>
   <BeginTime/>
   <EndTime/>
   <MaxItems/>
   <ReminderType/>
</GetReminders>

```

 <span data-ttu-id="3a06a-105">**жетреминдерстипе**</span><span class="sxs-lookup"><span data-stu-id="3a06a-105">**GetRemindersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a06a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3a06a-106">Attributes and elements</span></span>

<span data-ttu-id="3a06a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3a06a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a06a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3a06a-108">Attributes</span></span>

<span data-ttu-id="3a06a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3a06a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a06a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3a06a-110">Child elements</span></span>

<span data-ttu-id="3a06a-111">[Бегинтиме](begintime.md)  |  [EndTime (реминдермессажедататипе)](endtime-remindermessagedatatype.md)  |  [Макситемс](maxitems.md)  |  [Реминдертипе](remindertype.md)</span><span class="sxs-lookup"><span data-stu-id="3a06a-111">[BeginTime](begintime.md) | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md) | [MaxItems](maxitems.md) | [ReminderType](remindertype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a06a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3a06a-112">Parent elements</span></span>

<span data-ttu-id="3a06a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3a06a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a06a-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="3a06a-114">Remarks</span></span>

<span data-ttu-id="3a06a-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3a06a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a06a-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a06a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a06a-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3a06a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a06a-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3a06a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a06a-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3a06a-119">Schema Name</span></span>  <br/> |<span data-ttu-id="3a06a-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3a06a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a06a-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3a06a-121">Validation File</span></span>  <br/> |<span data-ttu-id="3a06a-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3a06a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a06a-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3a06a-123">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a06a-124">True</span><span class="sxs-lookup"><span data-stu-id="3a06a-124">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a06a-125">См. также</span><span class="sxs-lookup"><span data-stu-id="3a06a-125">See also</span></span>



- [<span data-ttu-id="3a06a-126">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3a06a-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

