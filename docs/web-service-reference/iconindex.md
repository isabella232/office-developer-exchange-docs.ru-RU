---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: Элемент IconIndex определяет индекс значка для элемента или беседы.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833848"
---
# <a name="iconindex"></a><span data-ttu-id="02a76-103">IconIndex</span><span class="sxs-lookup"><span data-stu-id="02a76-103">IconIndex</span></span>

<span data-ttu-id="02a76-104">Элемент **IconIndex** определяет индекс значка для элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="02a76-104">The **IconIndex** element identifies the icon index for an item or conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="02a76-105">**IconIndexType**</span><span class="sxs-lookup"><span data-stu-id="02a76-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="02a76-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="02a76-106">Attributes and elements</span></span>

<span data-ttu-id="02a76-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="02a76-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02a76-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="02a76-108">Attributes</span></span>

<span data-ttu-id="02a76-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="02a76-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02a76-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="02a76-110">Child elements</span></span>

<span data-ttu-id="02a76-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="02a76-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02a76-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="02a76-112">Parent elements</span></span>

<span data-ttu-id="02a76-113">[Беседы (ConversationType)](conversation-conversationtype.md) | [элемента](item.md) | [контакт](contact.md) | [DistributionList](distributionlist.md) | [сообщение](message-ex15websvcsotherref.md) | [элемента календаря, имеющего](calendaritem.md) | [PostItem](postitem.md) | [задач ](task.md)</span><span class="sxs-lookup"><span data-stu-id="02a76-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="02a76-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="02a76-114">Text value</span></span>

<span data-ttu-id="02a76-115">В следующей таблице приведены возможные значения для элемента **IconIndex** .</span><span class="sxs-lookup"><span data-stu-id="02a76-115">The following table contains the possible text values for the **IconIndex** element.</span></span> 
  
|<span data-ttu-id="02a76-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="02a76-116">**Value**</span></span>|<span data-ttu-id="02a76-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="02a76-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="02a76-118">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="02a76-118">Default</span></span>  <br/> |<span data-ttu-id="02a76-119">Указывает значок по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="02a76-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-120">PostItem</span><span class="sxs-lookup"><span data-stu-id="02a76-120">PostItem</span></span>  <br/> |<span data-ttu-id="02a76-121">Указывает значок для элемента записи.</span><span class="sxs-lookup"><span data-stu-id="02a76-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="02a76-122">MailRead</span><span class="sxs-lookup"><span data-stu-id="02a76-122">MailRead</span></span>  <br/> |<span data-ttu-id="02a76-123">Указывает, что значок чтения почты.</span><span class="sxs-lookup"><span data-stu-id="02a76-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-124">MailUnread</span><span class="sxs-lookup"><span data-stu-id="02a76-124">MailUnread</span></span>  <br/> |<span data-ttu-id="02a76-125">Указывает значок непрочитанных сообщений.</span><span class="sxs-lookup"><span data-stu-id="02a76-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-126">MailReplied</span><span class="sxs-lookup"><span data-stu-id="02a76-126">MailReplied</span></span>  <br/> |<span data-ttu-id="02a76-127">Задает пересылаемых значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-128">MailForwarded</span><span class="sxs-lookup"><span data-stu-id="02a76-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="02a76-129">Указывает значок пересылки почты.</span><span class="sxs-lookup"><span data-stu-id="02a76-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-130">MailEncrypted</span><span class="sxs-lookup"><span data-stu-id="02a76-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="02a76-131">Указывает значок зашифрованных сообщений.</span><span class="sxs-lookup"><span data-stu-id="02a76-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-132">MailSmimeSigned</span><span class="sxs-lookup"><span data-stu-id="02a76-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="02a76-133">Указывает значок подписью безопасные многоцелевые расширения почтового стандарта Интернета (S/MIME).</span><span class="sxs-lookup"><span data-stu-id="02a76-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-134">MailEncryptedReplied</span><span class="sxs-lookup"><span data-stu-id="02a76-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="02a76-135">Указывает, что зашифрованные ответ значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-136">MailSmimeSignedReplied</span><span class="sxs-lookup"><span data-stu-id="02a76-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="02a76-137">Указывает, что S/MIME подписанные пересылаемых значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-138">MailEncryptedForwarded</span><span class="sxs-lookup"><span data-stu-id="02a76-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="02a76-139">Указывает значок зашифрованных переадресованных сообщений.</span><span class="sxs-lookup"><span data-stu-id="02a76-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-140">MailSmimeSignedForwarded</span><span class="sxs-lookup"><span data-stu-id="02a76-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="02a76-141">Указывает, подписью S/MIME пересылку значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-142">MailEncryptedRead</span><span class="sxs-lookup"><span data-stu-id="02a76-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="02a76-143">Указывает значок зашифрованные чтения почты.</span><span class="sxs-lookup"><span data-stu-id="02a76-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-144">MailSmimeSignedRead</span><span class="sxs-lookup"><span data-stu-id="02a76-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="02a76-145">Указывает, подписью S/MIME чтение значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-146">MailIrm</span><span class="sxs-lookup"><span data-stu-id="02a76-146">MailIrm</span></span>  <br/> |<span data-ttu-id="02a76-147">Указывает значок Почта защищенного управления правами.</span><span class="sxs-lookup"><span data-stu-id="02a76-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-148">MailIrmForwarded</span><span class="sxs-lookup"><span data-stu-id="02a76-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="02a76-149">Указывает, защищенных службой IRM пересылку значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-150">MailIrmReplied</span><span class="sxs-lookup"><span data-stu-id="02a76-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="02a76-151">Указывает, что IRM-защитой дан ответ значок Почта.</span><span class="sxs-lookup"><span data-stu-id="02a76-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-152">SmsSubmitted</span><span class="sxs-lookup"><span data-stu-id="02a76-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="02a76-153">Указывает значок почты, отправленные на маршрутизации службы коротких сообщений (SMS).</span><span class="sxs-lookup"><span data-stu-id="02a76-153">Specifies the icon mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="02a76-154">SmsRoutedToDeliveryPoint</span><span class="sxs-lookup"><span data-stu-id="02a76-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="02a76-155">Указывает значок для SMS маршрутизации к точке внешних доставки.</span><span class="sxs-lookup"><span data-stu-id="02a76-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="02a76-156">SmsRoutedToExternalMessagingSystem</span><span class="sxs-lookup"><span data-stu-id="02a76-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="02a76-157">Указывает значок для маршрутизации SMS для внешней системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="02a76-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="02a76-158">SmsDelivered</span><span class="sxs-lookup"><span data-stu-id="02a76-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="02a76-159">Указывает значок доставлено почты SMS.</span><span class="sxs-lookup"><span data-stu-id="02a76-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-160">OutlookDefaultForContacts</span><span class="sxs-lookup"><span data-stu-id="02a76-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="02a76-161">Указывает значок по умолчанию для контактов.</span><span class="sxs-lookup"><span data-stu-id="02a76-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="02a76-162">AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="02a76-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="02a76-163">Указывает значок элемента встречи.</span><span class="sxs-lookup"><span data-stu-id="02a76-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-164">AppointmentRecur</span><span class="sxs-lookup"><span data-stu-id="02a76-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="02a76-165">Указывает значок повторяющейся встречи.</span><span class="sxs-lookup"><span data-stu-id="02a76-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-166">AppointmentMeet</span><span class="sxs-lookup"><span data-stu-id="02a76-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="02a76-167">Указывает значок собрания.</span><span class="sxs-lookup"><span data-stu-id="02a76-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-168">AppointmentMeetRecur</span><span class="sxs-lookup"><span data-stu-id="02a76-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="02a76-169">Указывает значок повторяющихся собраний.</span><span class="sxs-lookup"><span data-stu-id="02a76-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-170">AppointmentMeetNY</span><span class="sxs-lookup"><span data-stu-id="02a76-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="02a76-171">Указывает значок под вопросом ответа на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="02a76-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="02a76-172">AppointmentMeetYes</span><span class="sxs-lookup"><span data-stu-id="02a76-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="02a76-173">Указывает собрания значок приемки.</span><span class="sxs-lookup"><span data-stu-id="02a76-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-174">AppointmentMeetNo</span><span class="sxs-lookup"><span data-stu-id="02a76-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="02a76-175">Указывает значок отклоненные собрания.</span><span class="sxs-lookup"><span data-stu-id="02a76-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-176">AppointmentMeetMaybe</span><span class="sxs-lookup"><span data-stu-id="02a76-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="02a76-177">Указывает значок может быть ответа на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="02a76-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="02a76-178">AppointmentMeetCancel</span><span class="sxs-lookup"><span data-stu-id="02a76-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="02a76-179">Указывает значок Отменить собрание.</span><span class="sxs-lookup"><span data-stu-id="02a76-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-180">AppointmentMeetInfo</span><span class="sxs-lookup"><span data-stu-id="02a76-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="02a76-181">Указывает собрания значок информации.</span><span class="sxs-lookup"><span data-stu-id="02a76-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-182">TaskItem</span><span class="sxs-lookup"><span data-stu-id="02a76-182">TaskItem</span></span>  <br/> |<span data-ttu-id="02a76-183">Указывает значок элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="02a76-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-184">TaskRecur</span><span class="sxs-lookup"><span data-stu-id="02a76-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="02a76-185">Указывает значок повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="02a76-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-186">TaskOwned</span><span class="sxs-lookup"><span data-stu-id="02a76-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="02a76-187">Определяет задачу, владельцем которого значок.</span><span class="sxs-lookup"><span data-stu-id="02a76-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="02a76-188">TaskDelegated</span><span class="sxs-lookup"><span data-stu-id="02a76-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="02a76-189">Указывает значок делегированные задачи.</span><span class="sxs-lookup"><span data-stu-id="02a76-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="02a76-190">Замечания</span><span class="sxs-lookup"><span data-stu-id="02a76-190">Remarks</span></span>

<span data-ttu-id="02a76-191">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="02a76-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="02a76-192">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="02a76-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02a76-193">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="02a76-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02a76-194">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="02a76-194">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02a76-195">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="02a76-195">Schema name</span></span>  <br/> |<span data-ttu-id="02a76-196">Схема Types</span><span class="sxs-lookup"><span data-stu-id="02a76-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="02a76-197">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="02a76-197">Validation file</span></span>  <br/> |<span data-ttu-id="02a76-198">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="02a76-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="02a76-199">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="02a76-199">Can be empty</span></span>  <br/> |<span data-ttu-id="02a76-200">Нет</span><span class="sxs-lookup"><span data-stu-id="02a76-200">false</span></span>  <br/> |
   

