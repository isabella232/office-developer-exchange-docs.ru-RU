---
title: IconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92020822-2a86-4dfc-aee1-3067af4d4edf
description: Элемент Икониндекс определяет индекс значка для элемента или беседы.
ms.openlocfilehash: 8ada9da2df1cf128009c9b153736b434925f1a3f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833848"
---
# <a name="iconindex"></a><span data-ttu-id="64334-103">IconIndex</span><span class="sxs-lookup"><span data-stu-id="64334-103">IconIndex</span></span>

<span data-ttu-id="64334-104">Элемент **икониндекс** определяет индекс значка для элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="64334-104">The **IconIndex** element identifies the icon index for an item or conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MailIrmForwarded | MailIrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="64334-105">**икониндекстипе**</span><span class="sxs-lookup"><span data-stu-id="64334-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64334-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64334-106">Attributes and elements</span></span>

<span data-ttu-id="64334-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="64334-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64334-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64334-108">Attributes</span></span>

<span data-ttu-id="64334-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="64334-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64334-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64334-110">Child elements</span></span>

<span data-ttu-id="64334-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="64334-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="64334-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64334-112">Parent elements</span></span>

<span data-ttu-id="64334-113">[Беседа (конверсатионтипе)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [дистрибутионлист](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md)календаритем | Task i[Item](postitem.md) | [Task](task.md)</span><span class="sxs-lookup"><span data-stu-id="64334-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="64334-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="64334-114">Text value</span></span>

<span data-ttu-id="64334-115">В следующей таблице приведены возможные текстовые значения для элемента **икониндекс** .</span><span class="sxs-lookup"><span data-stu-id="64334-115">The following table contains the possible text values for the **IconIndex** element.</span></span> 
  
|<span data-ttu-id="64334-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="64334-116">**Value**</span></span>|<span data-ttu-id="64334-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64334-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="64334-118">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="64334-118">Default</span></span>  <br/> |<span data-ttu-id="64334-119">Задает значок по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="64334-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="64334-120">PostItem</span><span class="sxs-lookup"><span data-stu-id="64334-120">PostItem</span></span>  <br/> |<span data-ttu-id="64334-121">Задает значок элемента POST.</span><span class="sxs-lookup"><span data-stu-id="64334-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="64334-122">маилреад</span><span class="sxs-lookup"><span data-stu-id="64334-122">MailRead</span></span>  <br/> |<span data-ttu-id="64334-123">Указывает значок чтения почты.</span><span class="sxs-lookup"><span data-stu-id="64334-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="64334-124">маилунреад</span><span class="sxs-lookup"><span data-stu-id="64334-124">MailUnread</span></span>  <br/> |<span data-ttu-id="64334-125">Указывает значок непрочтенной почты.</span><span class="sxs-lookup"><span data-stu-id="64334-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-126">маилреплиед</span><span class="sxs-lookup"><span data-stu-id="64334-126">MailReplied</span></span>  <br/> |<span data-ttu-id="64334-127">Указывает значок "ответ на сообщение".</span><span class="sxs-lookup"><span data-stu-id="64334-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-128">маилфорвардед</span><span class="sxs-lookup"><span data-stu-id="64334-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="64334-129">Указывает значок переадресованной почты.</span><span class="sxs-lookup"><span data-stu-id="64334-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-130">маиленкриптед</span><span class="sxs-lookup"><span data-stu-id="64334-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="64334-131">Указывает значок зашифрованной почты.</span><span class="sxs-lookup"><span data-stu-id="64334-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-132">маилсмимесигнед</span><span class="sxs-lookup"><span data-stu-id="64334-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="64334-133">Указывает значок подписанного почтового расширения для безопасного или многоцелевого расширения почты в Интернете (S/MIME).</span><span class="sxs-lookup"><span data-stu-id="64334-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-134">маиленкриптедреплиед</span><span class="sxs-lookup"><span data-stu-id="64334-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="64334-135">Указывает зашифрованный значок, на который отправлен ответ.</span><span class="sxs-lookup"><span data-stu-id="64334-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-136">маилсмимесигнедреплиед</span><span class="sxs-lookup"><span data-stu-id="64334-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="64334-137">Указывает значок почтового ящика с подписанным сообщением S/MIME.</span><span class="sxs-lookup"><span data-stu-id="64334-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-138">маиленкриптедфорвардед</span><span class="sxs-lookup"><span data-stu-id="64334-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="64334-139">Указывает значок зашифрованной переадресованной почты.</span><span class="sxs-lookup"><span data-stu-id="64334-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-140">маилсмимесигнедфорвардед</span><span class="sxs-lookup"><span data-stu-id="64334-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="64334-141">Указывает значок переадресованного почтового ящика с подписью S/MIME.</span><span class="sxs-lookup"><span data-stu-id="64334-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-142">маиленкриптедреад</span><span class="sxs-lookup"><span data-stu-id="64334-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="64334-143">Задает зашифрованный значок чтения почты.</span><span class="sxs-lookup"><span data-stu-id="64334-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-144">маилсмимесигнедреад</span><span class="sxs-lookup"><span data-stu-id="64334-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="64334-145">Указывает подписанный значок чтения почты S/MIME.</span><span class="sxs-lookup"><span data-stu-id="64334-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-146">маилирм</span><span class="sxs-lookup"><span data-stu-id="64334-146">MailIrm</span></span>  <br/> |<span data-ttu-id="64334-147">Указывает значок защищенной службы управления правами на доступ к данным (IRM).</span><span class="sxs-lookup"><span data-stu-id="64334-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-148">маилирмфорвардед</span><span class="sxs-lookup"><span data-stu-id="64334-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="64334-149">Указывает значок переадресованной почты с защитой IRM.</span><span class="sxs-lookup"><span data-stu-id="64334-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-150">маилирмреплиед</span><span class="sxs-lookup"><span data-stu-id="64334-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="64334-151">Указывает значок почты, защищенный с помощью службы управления правами на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="64334-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-152">смссубмиттед</span><span class="sxs-lookup"><span data-stu-id="64334-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="64334-153">Указывает значок, отправленный для маршрутизации по протоколу коротких сообщений (SMS).</span><span class="sxs-lookup"><span data-stu-id="64334-153">Specifies the icon mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="64334-154">смсраутедтоделиверипоинт</span><span class="sxs-lookup"><span data-stu-id="64334-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="64334-155">Задает значок маршрутизации SMS для внешней точки доставки.</span><span class="sxs-lookup"><span data-stu-id="64334-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="64334-156">смсраутедтоекстерналмессагингсистем</span><span class="sxs-lookup"><span data-stu-id="64334-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="64334-157">Задает значок маршрутизации SMS для внешней системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="64334-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="64334-158">смсделиверед</span><span class="sxs-lookup"><span data-stu-id="64334-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="64334-159">Указывает значок доставленной почты SMS.</span><span class="sxs-lookup"><span data-stu-id="64334-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="64334-160">аутлукдефаултфорконтактс</span><span class="sxs-lookup"><span data-stu-id="64334-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="64334-161">Задает значок по умолчанию для контактов.</span><span class="sxs-lookup"><span data-stu-id="64334-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="64334-162">AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="64334-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="64334-163">Задает значок элемента встречи.</span><span class="sxs-lookup"><span data-stu-id="64334-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="64334-164">аппоинтментрекур</span><span class="sxs-lookup"><span data-stu-id="64334-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="64334-165">Задает значок повторяющейся встречи.</span><span class="sxs-lookup"><span data-stu-id="64334-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="64334-166">аппоинтментмит</span><span class="sxs-lookup"><span data-stu-id="64334-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="64334-167">Указывает значок собрания.</span><span class="sxs-lookup"><span data-stu-id="64334-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="64334-168">аппоинтментмитрекур</span><span class="sxs-lookup"><span data-stu-id="64334-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="64334-169">Задает значок повторяющегося собрания.</span><span class="sxs-lookup"><span data-stu-id="64334-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="64334-170">аппоинтментмитни</span><span class="sxs-lookup"><span data-stu-id="64334-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="64334-171">Задает значок ответа на приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="64334-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="64334-172">аппоинтментмитес</span><span class="sxs-lookup"><span data-stu-id="64334-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="64334-173">Указывает значок принятия приглашения на собрание.</span><span class="sxs-lookup"><span data-stu-id="64334-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="64334-174">аппоинтментмитно</span><span class="sxs-lookup"><span data-stu-id="64334-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="64334-175">Указывает значок "собрание отклонено".</span><span class="sxs-lookup"><span data-stu-id="64334-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="64334-176">аппоинтментмитмайбе</span><span class="sxs-lookup"><span data-stu-id="64334-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="64334-177">Задает значок, который может отреагировать на собрание.</span><span class="sxs-lookup"><span data-stu-id="64334-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="64334-178">аппоинтментмитканцел</span><span class="sxs-lookup"><span data-stu-id="64334-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="64334-179">Указывает значок отмены собрания.</span><span class="sxs-lookup"><span data-stu-id="64334-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="64334-180">аппоинтментмитинфо</span><span class="sxs-lookup"><span data-stu-id="64334-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="64334-181">Указывает значок сведений о собрании.</span><span class="sxs-lookup"><span data-stu-id="64334-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="64334-182">TaskItem</span><span class="sxs-lookup"><span data-stu-id="64334-182">TaskItem</span></span>  <br/> |<span data-ttu-id="64334-183">Задает значок элемента задачи.</span><span class="sxs-lookup"><span data-stu-id="64334-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="64334-184">таскрекур</span><span class="sxs-lookup"><span data-stu-id="64334-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="64334-185">Задает значок повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="64334-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="64334-186">тасковнед</span><span class="sxs-lookup"><span data-stu-id="64334-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="64334-187">Указывает значок владельца задачи.</span><span class="sxs-lookup"><span data-stu-id="64334-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="64334-188">таскделегатед</span><span class="sxs-lookup"><span data-stu-id="64334-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="64334-189">Задает делегированный значок задачи.</span><span class="sxs-lookup"><span data-stu-id="64334-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64334-190">Примечания</span><span class="sxs-lookup"><span data-stu-id="64334-190">Remarks</span></span>

<span data-ttu-id="64334-191">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="64334-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="64334-192">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="64334-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="64334-193">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64334-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64334-194">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64334-194">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64334-195">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64334-195">Schema name</span></span>  <br/> |<span data-ttu-id="64334-196">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64334-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="64334-197">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64334-197">Validation file</span></span>  <br/> |<span data-ttu-id="64334-198">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="64334-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64334-199">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64334-199">Can be empty</span></span>  <br/> |<span data-ttu-id="64334-200">false</span><span class="sxs-lookup"><span data-stu-id="64334-200">false</span></span>  <br/> |
   

