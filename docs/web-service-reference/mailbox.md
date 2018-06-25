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
description: Элемент почтового ящика идентифицирует почты объект Active Directory.
ms.openlocfilehash: e9fa21f3678249a9ac13d567b88beaf0177f989f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834258"
---
# <a name="mailbox"></a><span data-ttu-id="58e94-103">Почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="58e94-103">Mailbox</span></span>

<span data-ttu-id="58e94-104">Элемент **почтового ящика** идентифицирует почты объект Active Directory.</span><span class="sxs-lookup"><span data-stu-id="58e94-104">The **Mailbox** element identifies a mail-enabled Active Directory object.</span></span> 
  
```XML
<Mailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Mailbox>
```

<span data-ttu-id="58e94-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="58e94-105">**EmailAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="58e94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58e94-106">Attributes and elements</span></span>

<span data-ttu-id="58e94-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="58e94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58e94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58e94-108">Attributes</span></span>

<span data-ttu-id="58e94-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="58e94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58e94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58e94-110">Child elements</span></span>

|<span data-ttu-id="58e94-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e94-111">**Element**</span></span>|<span data-ttu-id="58e94-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e94-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e94-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="58e94-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="58e94-114">Определяет имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="58e94-114">Defines the name of the mailbox user.</span></span> <span data-ttu-id="58e94-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58e94-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58e94-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="58e94-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="58e94-117">Определяет адрес Simple Mail Transfer Protocol (SMTP) почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="58e94-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="58e94-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58e94-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58e94-119">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="58e94-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="58e94-120">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-120">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="58e94-121">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="58e94-121">The default is SMTP.</span></span> <span data-ttu-id="58e94-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58e94-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58e94-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="58e94-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="58e94-124">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-124">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="58e94-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58e94-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="58e94-126">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="58e94-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="58e94-127">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="58e94-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="58e94-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="58e94-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58e94-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58e94-129">Parent elements</span></span>

|<span data-ttu-id="58e94-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e94-130">**Element**</span></span>|<span data-ttu-id="58e94-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e94-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e94-132">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="58e94-132">ExpandDL</span></span>](expanddl.md) <br/> |<span data-ttu-id="58e94-133">Определяет запрос на разверните список рассылки.</span><span class="sxs-lookup"><span data-stu-id="58e94-133">Defines a request to expand a distribution list.</span></span> <br/> <br/> <span data-ttu-id="58e94-134">Ниже приведен выражение XPath для этого элемента.` /ExpandDL `</span><span class="sxs-lookup"><span data-stu-id="58e94-134">The following is the XPath expression to this element: ` /ExpandDL `</span></span> <br/> |
|[<span data-ttu-id="58e94-135">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="58e94-135">ToRecipients</span></span>](torecipients.md) <br/> |<span data-ttu-id="58e94-136">Содержит массив получателей элемента.</span><span class="sxs-lookup"><span data-stu-id="58e94-136">Contains an array of recipients of an item.</span></span>  <br/> |
|[<span data-ttu-id="58e94-137">CcRecipients</span><span class="sxs-lookup"><span data-stu-id="58e94-137">CcRecipients</span></span>](ccrecipients.md) <br/> |<span data-ttu-id="58e94-138">Представляет коллекцию получателей, которые будут получать копии сообщения.</span><span class="sxs-lookup"><span data-stu-id="58e94-138">Represents a collection of recipients that will receive a copy of the message.</span></span>  <br/> |
|[<span data-ttu-id="58e94-139">BccRecipients</span><span class="sxs-lookup"><span data-stu-id="58e94-139">BccRecipients</span></span>](bccrecipients.md) <br/> |<span data-ttu-id="58e94-140">Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="58e94-140">Represents a collection of recipients to receive a blind carbon copy (Bcc) of an e-mail.</span></span>  <br/> |
|[<span data-ttu-id="58e94-141">ReplyTo</span><span class="sxs-lookup"><span data-stu-id="58e94-141">ReplyTo</span></span>](replyto.md) <br/> |<span data-ttu-id="58e94-142">Определяет массив адресов электронной почты, на которые будут отправляться ответы.</span><span class="sxs-lookup"><span data-stu-id="58e94-142">Identifies an array of e-mail addresses to which replies should be sent.</span></span>  <br/> |
|[<span data-ttu-id="58e94-143">Отправитель</span><span class="sxs-lookup"><span data-stu-id="58e94-143">Sender</span></span>](sender.md) <br/> |<span data-ttu-id="58e94-144">Идентифицирует отправителя элемента.</span><span class="sxs-lookup"><span data-stu-id="58e94-144">Identifies the sender of an item.</span></span>  <br/> |
|[<span data-ttu-id="58e94-145">From</span><span class="sxs-lookup"><span data-stu-id="58e94-145">From</span></span>](from.md) <br/> |<span data-ttu-id="58e94-146">Представляет получателя, у которого было отправлено сообщение.</span><span class="sxs-lookup"><span data-stu-id="58e94-146">Represents the addressee from whom the message was sent.</span></span>  <br/> |
|[<span data-ttu-id="58e94-147">Организатор</span><span class="sxs-lookup"><span data-stu-id="58e94-147">Organizer</span></span>](organizer.md) <br/> |<span data-ttu-id="58e94-148">Представляет организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="58e94-148">Represents the organizer of a meeting.</span></span>  <br/> |
|[<span data-ttu-id="58e94-149">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="58e94-149">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> | <span data-ttu-id="58e94-150">Идентифицирует папок Microsoft Exchange Server 2007 по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="58e94-150">Identifies default Microsoft Exchange Server 2007 folders.</span></span>  <br/><br/>  <span data-ttu-id="58e94-151">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="58e94-151">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/CreateItem/ParentFolderId/DistinguishedFolderId` <br/>  `/CreateFolder/ParentFolderId/DistinguishedFolderId` <br/> |
|[<span data-ttu-id="58e94-152">Решение</span><span class="sxs-lookup"><span data-stu-id="58e94-152">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="58e94-153">Содержит одного объекта разрешения.</span><span class="sxs-lookup"><span data-stu-id="58e94-153">Contains a single resolved entity.</span></span>  <br/> |
|[<span data-ttu-id="58e94-154">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="58e94-154">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="58e94-155">Содержит массив почтовых ящиков, которые содержатся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="58e94-155">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="58e94-156">Attendee</span><span class="sxs-lookup"><span data-stu-id="58e94-156">Attendee</span></span>](attendee.md) <br/> |<span data-ttu-id="58e94-157">Представляет участников и ресурсов для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="58e94-157">Represents attendees and resources for a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="58e94-158">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="58e94-158">CreateManagedFolder</span></span>](createmanagedfolder.md) <br/> |<span data-ttu-id="58e94-159">Определяет запрос на добавление управляемых папок почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-159">Defines a request to add managed folders to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e94-160">Метод AddDelegate</span><span class="sxs-lookup"><span data-stu-id="58e94-160">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="58e94-161">Определяет запрос на Добавление делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="58e94-161">Defines a request to add delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e94-162">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="58e94-162">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="58e94-163">Определяет запрос на получение сведений о делегатов к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="58e94-163">Defines a request to get information about delegates to a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e94-164">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="58e94-164">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="58e94-165">Определяет запрос для удаления делегатов из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-165">Defines a request to remove delegates from a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e94-166">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="58e94-166">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="58e94-167">Определяет запрос на обновление делегаты в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="58e94-167">Defines a request to update delegates in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="58e94-168">Получил</span><span class="sxs-lookup"><span data-stu-id="58e94-168">ReceivedBy</span></span>](receivedby.md) <br/> |<span data-ttu-id="58e94-169">Описывает делегат в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="58e94-169">Describes the delegate in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="58e94-170">ReceivedRepresenting</span><span class="sxs-lookup"><span data-stu-id="58e94-170">ReceivedRepresenting</span></span>](receivedrepresenting.md) <br/> |<span data-ttu-id="58e94-171">Описывает участника в сценарии доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="58e94-171">Describes the principal in a delegate access scenario.</span></span>  <br/> |
|[<span data-ttu-id="58e94-172">Элемент</span><span class="sxs-lookup"><span data-stu-id="58e94-172">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="58e94-173">Представляет элемент в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="58e94-173">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="58e94-174">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="58e94-174">Text value</span></span>

<span data-ttu-id="58e94-175">Нет.</span><span class="sxs-lookup"><span data-stu-id="58e94-175">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="58e94-176">Замечания</span><span class="sxs-lookup"><span data-stu-id="58e94-176">Remarks</span></span>

<span data-ttu-id="58e94-177">Элементы [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) и [ItemId](itemid.md) определение списка рассылки или почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-177">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) and [ItemId](itemid.md) elements identify a mailbox or distribution list.</span></span> 

<span data-ttu-id="58e94-178">Элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) определяет почтовый ящик или список рассылки по SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="58e94-178">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element identifies a mailbox or distribution list by SMTP address.</span></span> 

<span data-ttu-id="58e94-179">Элемент [ItemId](itemid.md) идентифицирует почтового ящика, идентификатор элемента, который связан с определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="58e94-179">The [ItemId](itemid.md) element identifies a mailbox by an item identifier, which is associated with a particular mailbox.</span></span> 

<span data-ttu-id="58e94-180">Элемент [ItemId](itemid.md) не может использоваться для отправки сообщения в список рассылки и контактов в папке контактов общедоступной.</span><span class="sxs-lookup"><span data-stu-id="58e94-180">The [ItemId](itemid.md) element cannot be used for sending a message to a distribution list or a contact in a public contacts folder.</span></span> <span data-ttu-id="58e94-181">Ошибка возникает при использовании в ходе операции CreateItem, UpdateItem или SendItem при попытке отправить сообщение в список рассылки или контактов в общей папке контактов.</span><span class="sxs-lookup"><span data-stu-id="58e94-181">An error will be thrown if this is used in a CreateItem, UpdateItem, or SendItem operation when an attempt is made to send a message to a distribution list or contact in a contacts public folder.</span></span> <span data-ttu-id="58e94-182">Используйте операцию ExpandDL для получения SMTP-адрес и отправьте сообщение с помощью элемента [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) вместо [ItemId](itemid.md) элемент.</span><span class="sxs-lookup"><span data-stu-id="58e94-182">Use the ExpandDL operation to get the SMTP address and then send the message by using the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element instead of the [ItemId](itemid.md) element.</span></span> 
  
<span data-ttu-id="58e94-183">Другого элемента [почтового ящика (доступность)](mailbox-availability.md), сведения о доступности операций.</span><span class="sxs-lookup"><span data-stu-id="58e94-183">Another element, [Mailbox (Availability)](mailbox-availability.md), provides information for availability operations.</span></span> 
  
<span data-ttu-id="58e94-184">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="58e94-184">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58e94-185">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58e94-185">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58e94-186">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58e94-186">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58e94-187">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58e94-187">Schema Name</span></span>  <br/> |<span data-ttu-id="58e94-188">Схема Types</span><span class="sxs-lookup"><span data-stu-id="58e94-188">Types schema</span></span>  <br/> |
|<span data-ttu-id="58e94-189">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58e94-189">Validation File</span></span>  <br/> |<span data-ttu-id="58e94-190">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="58e94-190">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="58e94-191">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58e94-191">Can be Empty</span></span>  <br/> |<span data-ttu-id="58e94-192">False</span><span class="sxs-lookup"><span data-stu-id="58e94-192">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58e94-193">См. также</span><span class="sxs-lookup"><span data-stu-id="58e94-193">See also</span></span>

- [<span data-ttu-id="58e94-194">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="58e94-194">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

