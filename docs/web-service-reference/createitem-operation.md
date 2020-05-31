---
title: Операция CreateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 78a52120-f1d0-4ed7-8748-436e554f75b6
description: Операция CreateItem создает элементы в хранилище Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761897"
---
# <a name="createitem-operation"></a><span data-ttu-id="0dcbe-103">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="0dcbe-103">CreateItem operation</span></span>

<span data-ttu-id="0dcbe-104">Операция CreateItem создает элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="0dcbe-105">Использование операции CreateItem</span><span class="sxs-lookup"><span data-stu-id="0dcbe-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="0dcbe-106">С помощью операции CreateItem можно создать следующее:</span><span class="sxs-lookup"><span data-stu-id="0dcbe-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="0dcbe-107">Элементы календаря</span><span class="sxs-lookup"><span data-stu-id="0dcbe-107">Calendar items</span></span>
    
- <span data-ttu-id="0dcbe-108">Сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="0dcbe-108">E-mail messages</span></span>
    
- <span data-ttu-id="0dcbe-109">Приглашения на собрания</span><span class="sxs-lookup"><span data-stu-id="0dcbe-109">Meeting requests</span></span>
    
- <span data-ttu-id="0dcbe-110">Задачи</span><span class="sxs-lookup"><span data-stu-id="0dcbe-110">Tasks</span></span>
    
- <span data-ttu-id="0dcbe-111">Контакты</span><span class="sxs-lookup"><span data-stu-id="0dcbe-111">Contacts</span></span>
    
<span data-ttu-id="0dcbe-112">Для получения дополнительных сведений см. [Операция CreateItem (элемент календаря)](createitem-operation-calendar-item.md), [Операция CreateItem (сообщение электронной почты)](createitem-operation-email-message.md), [Операция CreateItem (приглашение на собрание)](createitem-operation-meeting-request.md), [Операция CreateItem (Task)](createitem-operation-task.md)и [Операция CreateItem (Contact)](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="0dcbe-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="0dcbe-113">Операция CreateItem поддерживает использование объектов Response.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="0dcbe-114">Объекты Response поддерживают принятие и отклонение собраний и обработку кнопок голосования, включенных в стандартное электронное сообщение.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="0dcbe-115">В следующей таблице перечислены объекты ответа, которые обрабатываются в операции CreateItem.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="0dcbe-116">**Объект Response**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-116">**Response object**</span></span>|<span data-ttu-id="0dcbe-117">**Действие**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0dcbe-118">акцептитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="0dcbe-119">Принятие приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-120">канцелкалендаритем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="0dcbe-121">Отмена собрания.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-121">Cancel a meeting.</span></span> <span data-ttu-id="0dcbe-122">Это отличается от удаления всех участников, так как он также удаляет собрание для организатора.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-123">деклинеитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="0dcbe-124">Отклонение приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-125">форвардитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="0dcbe-126">Отправка приглашения на собрание другому человеку в качестве приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="0dcbe-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="0dcbe-128">Удаление отмененного собрания из календаря.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-129">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="0dcbe-130">Отправьте сообщение, содержащее текст исходного приглашения на собрание всем участникам собрания.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-131">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="0dcbe-132">Отправьте сообщение, содержащее текст исходного приглашения на собрание отправителю приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-133">сендреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="0dcbe-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="0dcbe-134">Отправка уведомления о прочтении отправителю приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-135">тентативелякцептитем</span><span class="sxs-lookup"><span data-stu-id="0dcbe-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="0dcbe-136">Принятие приглашения на собрание под вопросом.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="0dcbe-137">Операция CreateItem также поддерживает дополнительные объекты Meeting.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="0dcbe-138">В следующей таблице перечислены дополнительные объекты, поддерживаемые операцией CreateItem.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="0dcbe-139">**Объект Meeting**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-139">**Meeting object**</span></span>|<span data-ttu-id="0dcbe-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0dcbe-141">Сообщение о собрании</span><span class="sxs-lookup"><span data-stu-id="0dcbe-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="0dcbe-142">Представляет сообщение о собрании в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="0dcbe-143">Это базовый объект для других объектов Meeting.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-144">Приглашение на собрание</span><span class="sxs-lookup"><span data-stu-id="0dcbe-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="0dcbe-145">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-146">Ответ на приглашение на собрание</span><span class="sxs-lookup"><span data-stu-id="0dcbe-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="0dcbe-147">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="0dcbe-148">Отмена собрания</span><span class="sxs-lookup"><span data-stu-id="0dcbe-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="0dcbe-149">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0dcbe-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dcbe-150">См. также</span><span class="sxs-lookup"><span data-stu-id="0dcbe-150">See also</span></span>



[<span data-ttu-id="0dcbe-151">Операция CreateItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="0dcbe-152">Операция CreateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="0dcbe-153">Операция CreateItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="0dcbe-154">Операция CreateItem (приглашение на собрание)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="0dcbe-155">Операция CreateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="0dcbe-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="0dcbe-156">**креатеитемтипе**</span><span class="sxs-lookup"><span data-stu-id="0dcbe-156">**CreateItemType**</span></span>

