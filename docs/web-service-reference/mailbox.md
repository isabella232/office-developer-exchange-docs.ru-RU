---
title: Почтовый ящик
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: befc70fd-51cb-4258-884c-80c9050f0e82
description: Элемент Mailbox определяет объект Active Directory с включенной поддержкой почты.
ms.openlocfilehash: 284c3ff6f9fece57611169a4ec41eeaa273c6ad3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468203"
---
# <a name="mailbox"></a><span data-ttu-id="d3aa2-103">Почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="d3aa2-103">Mailbox</span></span>

<span data-ttu-id="d3aa2-104">Элемент **Mailbox** определяет объект Active Directory с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="d3aa2-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="d3aa2-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d3aa2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3aa2-106">Attributes and elements</span></span>

<span data-ttu-id="d3aa2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3aa2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3aa2-108">Attributes</span></span>

<span data-ttu-id="d3aa2-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3aa2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3aa2-110">Child elements</span></span>

|<span data-ttu-id="d3aa2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3aa2-111">**Element**</span></span>|<span data-ttu-id="d3aa2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3aa2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3aa2-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d3aa2-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="d3aa2-114">Определяет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="d3aa2-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="d3aa2-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="d3aa2-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="d3aa2-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="d3aa2-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="d3aa2-120">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="d3aa2-121">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-121">The default is SMTP.</span></span> <span data-ttu-id="d3aa2-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="d3aa2-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="d3aa2-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="d3aa2-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="d3aa2-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d3aa2-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="d3aa2-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3aa2-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3aa2-129">Parent elements</span></span>

|<span data-ttu-id="d3aa2-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3aa2-130">**Element**</span></span>|<span data-ttu-id="d3aa2-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3aa2-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3aa2-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="d3aa2-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="d3aa2-133">Определяет запрос на развертывание списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="d3aa2-134">Ниже приведено выражение XPath для этого элемента:` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="d3aa2-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="d3aa2-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d3aa2-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="d3aa2-136">Содержит массив получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="d3aa2-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="d3aa2-138">Представляет коллекцию получателей, которые будут получать копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="d3aa2-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="d3aa2-140">Представляет коллекцию получателей для получения скрытой копии сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="d3aa2-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="d3aa2-142">Определяет массив адресов электронной почты, в которые должны отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-143">Sender</span><span class="sxs-lookup"><span data-stu-id="d3aa2-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="d3aa2-144">Определяет отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-145">From</span><span class="sxs-lookup"><span data-stu-id="d3aa2-145">From</span></span>](from.md) <br/> |<span data-ttu-id="d3aa2-146">Представляет адрес получателя, от которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-147">Organizer</span><span class="sxs-lookup"><span data-stu-id="d3aa2-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="d3aa2-148">Представляет организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-149">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="d3aa2-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="d3aa2-150">Определяет стандартные папки Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="d3aa2-151">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="d3aa2-152">Resolution</span><span class="sxs-lookup"><span data-stu-id="d3aa2-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="d3aa2-153">Содержит одну разрешенную сущность.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-154">длекспансион</span><span class="sxs-lookup"><span data-stu-id="d3aa2-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="d3aa2-155">Содержит массив почтовых ящиков, содержащихся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-156">Участник</span><span class="sxs-lookup"><span data-stu-id="d3aa2-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="d3aa2-157">Представляет участников и ресурсы для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="d3aa2-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="d3aa2-159">Определяет запрос на добавление управляемых папок в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-160">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="d3aa2-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="d3aa2-161">Определяет запрос на добавление делегатов в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="d3aa2-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="d3aa2-163">Определяет запрос на получение сведений о делегатах для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="d3aa2-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="d3aa2-165">Определяет запрос на удаление делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="d3aa2-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="d3aa2-167">Определяет запрос на обновление делегатов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-168">рецеиведби</span><span class="sxs-lookup"><span data-stu-id="d3aa2-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="d3aa2-169">Описывает делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-170">рецеиведрепресентинг</span><span class="sxs-lookup"><span data-stu-id="d3aa2-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="d3aa2-171">Описывает участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="d3aa2-172">Элемент</span><span class="sxs-lookup"><span data-stu-id="d3aa2-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d3aa2-173">Представляет члена списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3aa2-174">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d3aa2-174">Text value</span></span>

<span data-ttu-id="d3aa2-175">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3aa2-176">Примечания</span><span class="sxs-lookup"><span data-stu-id="d3aa2-176">Remarks</span></span>

<span data-ttu-id="d3aa2-177">Элементы [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) и [ItemId](itemid.md) идентифицируют почтовый ящик или список рассылки.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="d3aa2-178">Элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) определяет почтовый ящик или список рассылки по SMTP-адресу.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="d3aa2-179">Элемент [ItemId](itemid.md) идентифицирует почтовый ящик по идентификатору элемента, связанному с определенным почтовым ящиком.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="d3aa2-180">Элемент [ItemId](itemid.md) нельзя использовать для отправки сообщения в список рассылки или контакт в общедоступной папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="d3aa2-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="d3aa2-181">Если при попытке отправить сообщение в список рассылки или контакт в общедоступной папке Contacts, будет выдаваться сообщение об ошибке, если оно используется в операции CreateItem, UpdateItem или SendItem.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="d3aa2-182">Используйте операцию ExpandDL для получения SMTP-адреса, а затем отправьте сообщение с помощью элемента [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) , а не элемента [ItemId](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="d3aa2-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="d3aa2-183">Другой элемент, [Mailbox (Availability)](mailbox-availability.md), предоставляет сведения об операциях обеспечения доступности.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="d3aa2-184">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3aa2-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3aa2-185">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3aa2-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3aa2-186">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3aa2-186">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3aa2-187">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3aa2-187">Schema Name</span></span>  <br/> |<span data-ttu-id="d3aa2-188">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3aa2-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3aa2-189">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3aa2-189">Validation File</span></span>  <br/> |<span data-ttu-id="d3aa2-190">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d3aa2-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3aa2-191">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3aa2-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3aa2-192">False</span><span class="sxs-lookup"><span data-stu-id="d3aa2-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3aa2-193">См. также</span><span class="sxs-lookup"><span data-stu-id="d3aa2-193">See also</span></span>

- [<span data-ttu-id="d3aa2-194">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d3aa2-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

