---
title: CreateItem Operation
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
description: Операции CreateItem создает элементов в хранилище Exchange.
ms.openlocfilehash: 7e1808c685cdbaa1e8867aa7425b2cc52218d001
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761897"
---
# <a name="createitem-operation"></a><span data-ttu-id="21676-103">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="21676-103">CreateItem operation</span></span>

<span data-ttu-id="21676-104">Операции CreateItem создает элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="21676-104">The CreateItem operation creates items in the Exchange store.</span></span>
  
## <a name="using-the-createitem-operation"></a><span data-ttu-id="21676-105">С помощью операции CreateItem</span><span class="sxs-lookup"><span data-stu-id="21676-105">Using the CreateItem Operation</span></span>

<span data-ttu-id="21676-106">Можно использовать операцию CreateItem для создания следующих:</span><span class="sxs-lookup"><span data-stu-id="21676-106">You can use the CreateItem operation to create the following:</span></span>
  
- <span data-ttu-id="21676-107">Элементы календаря</span><span class="sxs-lookup"><span data-stu-id="21676-107">Calendar items</span></span>
    
- <span data-ttu-id="21676-108">Сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="21676-108">E-mail messages</span></span>
    
- <span data-ttu-id="21676-109">Приглашения на собрания</span><span class="sxs-lookup"><span data-stu-id="21676-109">Meeting requests</span></span>
    
- <span data-ttu-id="21676-110">Задачи</span><span class="sxs-lookup"><span data-stu-id="21676-110">Tasks</span></span>
    
- <span data-ttu-id="21676-111">Контакты</span><span class="sxs-lookup"><span data-stu-id="21676-111">Contacts</span></span>
    
<span data-ttu-id="21676-112">Для получения дополнительных сведений см [операции CreateItem (элемента календаря)](createitem-operation-calendar-item.md), [операции CreateItem (сообщение электронной почты)](createitem-operation-email-message.md), [операции CreateItem (собрание)](createitem-operation-meeting-request.md), [операции CreateItem (задача)](createitem-operation-task.md)и [операции CreateItem (контактов) ](createitem-operation-contact.md).</span><span class="sxs-lookup"><span data-stu-id="21676-112">For more information, see [CreateItem operation (calendar item)](createitem-operation-calendar-item.md), [CreateItem operation (email message)](createitem-operation-email-message.md), [CreateItem operation (meeting request)](createitem-operation-meeting-request.md), [CreateItem operation (task)](createitem-operation-task.md), and [CreateItem operation (contact)](createitem-operation-contact.md).</span></span>
  
<span data-ttu-id="21676-113">Операции CreateItem поддерживает использование объекты ответа.</span><span class="sxs-lookup"><span data-stu-id="21676-113">The CreateItem operation supports the use of response objects.</span></span> <span data-ttu-id="21676-114">Объекты ответа поддерживает приемки и отклонения собраний и обработки кнопки голосования, которые включены в стандартные электронные сообщения.</span><span class="sxs-lookup"><span data-stu-id="21676-114">Response objects support the acceptance and rejection of meetings and the handling of voting buttons that are included in a standard e-mail message.</span></span> <span data-ttu-id="21676-115">В следующей таблице перечислены объекты ответа, которые обрабатываются в операции CreateItem.</span><span class="sxs-lookup"><span data-stu-id="21676-115">The following table lists the response objects that are handled in the CreateItem operation.</span></span>
  
|<span data-ttu-id="21676-116">**Объект ответа**</span><span class="sxs-lookup"><span data-stu-id="21676-116">**Response object**</span></span>|<span data-ttu-id="21676-117">**Действие**</span><span class="sxs-lookup"><span data-stu-id="21676-117">**Action**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21676-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="21676-118">AcceptItem</span></span>  <br/> |<span data-ttu-id="21676-119">Принятие приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-119">Accept a meeting request.</span></span>  <br/> |
|<span data-ttu-id="21676-120">CancelCalendarItem</span><span class="sxs-lookup"><span data-stu-id="21676-120">CancelCalendarItem</span></span>  <br/> |<span data-ttu-id="21676-121">Отмена собрания.</span><span class="sxs-lookup"><span data-stu-id="21676-121">Cancel a meeting.</span></span> <span data-ttu-id="21676-122">Это отличается от удаления всех участников, так как он также удаляет для организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="21676-122">This differs from deleting all attendees because it deletes the meeting for the organizer also.</span></span>  <br/> |
|<span data-ttu-id="21676-123">DeclineItem</span><span class="sxs-lookup"><span data-stu-id="21676-123">DeclineItem</span></span>  <br/> |<span data-ttu-id="21676-124">Отклонение приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-124">Decline a meeting request.</span></span>  <br/> |
|<span data-ttu-id="21676-125">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="21676-125">ForwardItem</span></span>  <br/> |<span data-ttu-id="21676-126">Отправьте приглашения на собрание другому пользователю в виде приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-126">Send a meeting request to another person as a meeting request.</span></span>  <br/> |
|<span data-ttu-id="21676-127">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="21676-127">RemoveItem</span></span>  <br/> |<span data-ttu-id="21676-128">Удалите отмененные собрания из календаря.</span><span class="sxs-lookup"><span data-stu-id="21676-128">Remove a canceled meeting from the calendar.</span></span>  <br/> |
|<span data-ttu-id="21676-129">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="21676-129">ReplyAllToItem</span></span>  <br/> |<span data-ttu-id="21676-130">Отправьте сообщение, содержащее текст исходного запроса на проведение собрания всем участникам собрания.</span><span class="sxs-lookup"><span data-stu-id="21676-130">Send a message that includes the body of the original meeting request to all attendees of the meeting.</span></span>  <br/> |
|<span data-ttu-id="21676-131">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="21676-131">ReplyToItem</span></span>  <br/> |<span data-ttu-id="21676-132">Отправьте сообщение, содержащее текст исходного запроса на проведение собрания отправителю приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-132">Send a message that includes the body of the original meeting request to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="21676-133">SendReadReceipt</span><span class="sxs-lookup"><span data-stu-id="21676-133">SendReadReceipt</span></span>  <br/> |<span data-ttu-id="21676-134">Отправьте уведомление отправителю приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-134">Send a read receipt to the sender of the meeting request.</span></span>  <br/> |
|<span data-ttu-id="21676-135">TentativelyAcceptItem</span><span class="sxs-lookup"><span data-stu-id="21676-135">TentativelyAcceptItem</span></span>  <br/> |<span data-ttu-id="21676-136">Предварительное принятие приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="21676-136">Tentatively accept a meeting request.</span></span>  <br/> |
   
<span data-ttu-id="21676-137">Операции CreateItem также поддерживает дополнительных объектов.</span><span class="sxs-lookup"><span data-stu-id="21676-137">The CreateItem operation also supports additional meeting objects.</span></span> <span data-ttu-id="21676-138">В следующей таблице перечислены дополнительные объекты, поддерживаемые операции CreateItem.</span><span class="sxs-lookup"><span data-stu-id="21676-138">The following table lists additional objects that the CreateItem operation supports.</span></span>
  
|<span data-ttu-id="21676-139">**Объект собрания**</span><span class="sxs-lookup"><span data-stu-id="21676-139">**Meeting object**</span></span>|<span data-ttu-id="21676-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="21676-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21676-141">Сообщения о собрании</span><span class="sxs-lookup"><span data-stu-id="21676-141">Meeting Message</span></span>  <br/> |<span data-ttu-id="21676-142">Представляет сообщение собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="21676-142">Represents a meeting message in the Exchange store.</span></span> <span data-ttu-id="21676-143">Это базовый объект для других объектов собрания.</span><span class="sxs-lookup"><span data-stu-id="21676-143">This is the base object for the other meeting objects.</span></span>  <br/> |
|<span data-ttu-id="21676-144">Приглашения на собрание</span><span class="sxs-lookup"><span data-stu-id="21676-144">Meeting Request</span></span>  <br/> |<span data-ttu-id="21676-145">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="21676-145">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="21676-146">Приглашения на собрание</span><span class="sxs-lookup"><span data-stu-id="21676-146">Meeting Response</span></span>  <br/> |<span data-ttu-id="21676-147">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="21676-147">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="21676-148">Отмена собрания</span><span class="sxs-lookup"><span data-stu-id="21676-148">Meeting Cancellation</span></span>  <br/> |<span data-ttu-id="21676-149">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="21676-149">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21676-150">См. также</span><span class="sxs-lookup"><span data-stu-id="21676-150">See also</span></span>



[<span data-ttu-id="21676-151">Операции CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="21676-151">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)
  
[<span data-ttu-id="21676-152">Операции CreateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="21676-152">CreateItem operation (contact)</span></span>](createitem-operation-contact.md)
  
[<span data-ttu-id="21676-153">Операции CreateItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="21676-153">CreateItem operation (email message)</span></span>](createitem-operation-email-message.md)
  
[<span data-ttu-id="21676-154">Операции CreateItem (запрос на собрание)</span><span class="sxs-lookup"><span data-stu-id="21676-154">CreateItem operation (meeting request)</span></span>](createitem-operation-meeting-request.md)
  
[<span data-ttu-id="21676-155">Операции CreateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="21676-155">CreateItem operation (task)</span></span>](createitem-operation-task.md)
  
 <span data-ttu-id="21676-156">**CreateItemType**</span><span class="sxs-lookup"><span data-stu-id="21676-156">**CreateItemType**</span></span>

