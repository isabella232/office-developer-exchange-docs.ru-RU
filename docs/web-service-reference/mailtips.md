---
title: Подсказки
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: Элемент подсказки представляет значения для различных типов советов по использованию электронной почты.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44447598"
---
# <a name="mailtips"></a><span data-ttu-id="d3835-103">Подсказки</span><span class="sxs-lookup"><span data-stu-id="d3835-103">MailTips</span></span>

<span data-ttu-id="d3835-104">Элемент **подсказки** представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d3835-104">The **MailTips** element represents values for various types of mail tips.</span></span> 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 <span data-ttu-id="d3835-105">**Подсказки**</span><span class="sxs-lookup"><span data-stu-id="d3835-105">**MailTips**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3835-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3835-106">Attributes and elements</span></span>

<span data-ttu-id="d3835-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d3835-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3835-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3835-108">Attributes</span></span>

<span data-ttu-id="d3835-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d3835-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3835-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3835-110">Child elements</span></span>

|<span data-ttu-id="d3835-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3835-111">**Element**</span></span>|<span data-ttu-id="d3835-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3835-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3835-113">RecipientAddress</span><span class="sxs-lookup"><span data-stu-id="d3835-113">RecipientAddress</span></span>](recipientaddress.md) <br/> |<span data-ttu-id="d3835-114">Представляет почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="d3835-114">Represents the mailbox of the recipient.</span></span>  <br/> |
|[<span data-ttu-id="d3835-115">пендингмаилтипс</span><span class="sxs-lookup"><span data-stu-id="d3835-115">PendingMailTips</span></span>](pendingmailtips.md) <br/> |<span data-ttu-id="d3835-116">Указывает, что советы по использованию электронной почты в этом элементе невозможно оценить до истечения времени ожидания обработки на сервере.</span><span class="sxs-lookup"><span data-stu-id="d3835-116">Indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span>  <br/> |
|[<span data-ttu-id="d3835-117">аутофоффице</span><span class="sxs-lookup"><span data-stu-id="d3835-117">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="d3835-118">Представляет ответное сообщение и время для отправки ответного сообщения.</span><span class="sxs-lookup"><span data-stu-id="d3835-118">Represents the response message and a duration time for sending the response message.</span></span>  <br/> |
|[<span data-ttu-id="d3835-119">маилбоксфулл</span><span class="sxs-lookup"><span data-stu-id="d3835-119">MailboxFull</span></span>](mailboxfull.md) <br/> |<span data-ttu-id="d3835-120">Указывает, заполнен ли почтовый ящик получателя.</span><span class="sxs-lookup"><span data-stu-id="d3835-120">Indicates whether the mailbox for the recipient is full.</span></span>  <br/> |
|[<span data-ttu-id="d3835-121">кустоммаилтип</span><span class="sxs-lookup"><span data-stu-id="d3835-121">CustomMailTip</span></span>](custommailtip.md) <br/> |<span data-ttu-id="d3835-122">Представляет настраиваемое сообщение подсказки.</span><span class="sxs-lookup"><span data-stu-id="d3835-122">Represents a customized mail tip message.</span></span>  <br/> |
|[<span data-ttu-id="d3835-123">тоталмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="d3835-123">TotalMemberCount</span></span>](totalmembercount.md) <br/> |<span data-ttu-id="d3835-124">Представляет количество всех элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="d3835-124">Represents the count of all members in a group.</span></span>  <br/> |
|[<span data-ttu-id="d3835-125">екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="d3835-125">ExternalMemberCount</span></span>](externalmembercount.md) <br/> |<span data-ttu-id="d3835-126">Представляет количество внешних элементов в группе.</span><span class="sxs-lookup"><span data-stu-id="d3835-126">Represents the count of external members in a group.</span></span>  <br/> |
|[<span data-ttu-id="d3835-127">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="d3835-127">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="d3835-128">Представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="d3835-128">Represents the maximum message size the recipient can accept.</span></span>  <br/> |
|[<span data-ttu-id="d3835-129">деливерирестриктед</span><span class="sxs-lookup"><span data-stu-id="d3835-129">DeliveryRestricted</span></span>](deliveryrestricted.md) <br/> |<span data-ttu-id="d3835-130">Указывает, будут ли ограничения доставки допустить достижение получателю сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="d3835-130">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|[<span data-ttu-id="d3835-131">Модератор</span><span class="sxs-lookup"><span data-stu-id="d3835-131">IsModerated</span></span>](ismoderated.md) <br/> |<span data-ttu-id="d3835-132">Указывает, является ли почтовый ящик получателя ведущим.</span><span class="sxs-lookup"><span data-stu-id="d3835-132">Indicates whether the recipient's mailbox is being moderated.</span></span>  <br/> |
|[<span data-ttu-id="d3835-133">ИнвалидреЦипиент (подсказки)</span><span class="sxs-lookup"><span data-stu-id="d3835-133">InvalidRecipient (MailTips)</span></span>](invalidrecipient-mailtips.md) <br/> |<span data-ttu-id="d3835-134">Указывает, является ли получатель недопустимым.</span><span class="sxs-lookup"><span data-stu-id="d3835-134">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3835-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3835-135">Parent elements</span></span>

|<span data-ttu-id="d3835-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3835-136">**Element**</span></span>|<span data-ttu-id="d3835-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3835-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3835-138">маилтипсреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="d3835-138">MailTipsResponseMessageType</span></span>](mailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="d3835-139">Представляет параметры почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="d3835-139">Represents mail tips settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3835-140">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d3835-140">Text value</span></span>

<span data-ttu-id="d3835-141">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3835-141">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3835-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="d3835-142">Remarks</span></span>

<span data-ttu-id="d3835-143">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3835-143">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3835-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3835-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3835-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3835-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d3835-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3835-146">Schema Name</span></span>  <br/> |<span data-ttu-id="d3835-147">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d3835-147">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d3835-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3835-148">Validation File</span></span>  <br/> |<span data-ttu-id="d3835-149">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d3835-149">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d3835-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3835-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3835-151">False</span><span class="sxs-lookup"><span data-stu-id="d3835-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3835-152">См. также</span><span class="sxs-lookup"><span data-stu-id="d3835-152">See also</span></span>



- [<span data-ttu-id="d3835-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d3835-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

