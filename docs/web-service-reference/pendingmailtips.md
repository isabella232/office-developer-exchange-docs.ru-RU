---
title: пендингмаилтипс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: Элемент Пендингмаилтипс указывает на то, что советы по использованию электронной почты в этом элементе невозможно оценить до истечения времени ожидания обработки на сервере.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834704"
---
# <a name="pendingmailtips"></a><span data-ttu-id="1dc27-103">пендингмаилтипс</span><span class="sxs-lookup"><span data-stu-id="1dc27-103">PendingMailTips</span></span>

<span data-ttu-id="1dc27-104">Элемент **пендингмаилтипс** указывает на то, что советы по использованию электронной почты в этом элементе невозможно оценить до истечения времени ожидания обработки на сервере.</span><span class="sxs-lookup"><span data-stu-id="1dc27-104">The **PendingMailTips** element indicates that the mail tips in this element could not be evaluated before the server's processing timeout expired.</span></span> 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 <span data-ttu-id="1dc27-105">**маилтиптипес**</span><span class="sxs-lookup"><span data-stu-id="1dc27-105">**MailTipTypes**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dc27-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1dc27-106">Attributes and elements</span></span>

<span data-ttu-id="1dc27-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1dc27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dc27-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1dc27-108">Attributes</span></span>

<span data-ttu-id="1dc27-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1dc27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dc27-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1dc27-110">Child elements</span></span>

<span data-ttu-id="1dc27-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1dc27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1dc27-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1dc27-112">Parent elements</span></span>

|<span data-ttu-id="1dc27-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1dc27-113">**Element**</span></span>|<span data-ttu-id="1dc27-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1dc27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dc27-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="1dc27-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="1dc27-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1dc27-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1dc27-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1dc27-117">Text value</span></span>

<span data-ttu-id="1dc27-118">В следующей таблице приведены возможные значения для элемента **пендингмаилтипс** .</span><span class="sxs-lookup"><span data-stu-id="1dc27-118">The following table lists the possible values for the **PendingMailTips** element.</span></span> 
  
|<span data-ttu-id="1dc27-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="1dc27-119">**Value**</span></span>|<span data-ttu-id="1dc27-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1dc27-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1dc27-121">Все</span><span class="sxs-lookup"><span data-stu-id="1dc27-121">All</span></span>  <br/> |<span data-ttu-id="1dc27-122">Представляет все доступные советы по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1dc27-122">Represents all available mail tips.</span></span>  <br/> |
|<span data-ttu-id="1dc27-123">аутофоффицемессаже</span><span class="sxs-lookup"><span data-stu-id="1dc27-123">OutOfOfficeMessage</span></span>  <br/> |<span data-ttu-id="1dc27-124">Представляет сообщение об отсутствии на рабочем месте (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="1dc27-124">Represents the Out of Office (OOF) message.</span></span>  <br/> |
|<span data-ttu-id="1dc27-125">маилбоксфуллстатус</span><span class="sxs-lookup"><span data-stu-id="1dc27-125">MailboxFullStatus</span></span>  <br/> |<span data-ttu-id="1dc27-126">Представляет состояние для почтового ящика Full.</span><span class="sxs-lookup"><span data-stu-id="1dc27-126">Represents the status for a mailbox being full.</span></span>  <br/> |
|<span data-ttu-id="1dc27-127">кустоммаилтип</span><span class="sxs-lookup"><span data-stu-id="1dc27-127">CustomMailTip</span></span>  <br/> |<span data-ttu-id="1dc27-128">Представляет настраиваемую подсказку почты.</span><span class="sxs-lookup"><span data-stu-id="1dc27-128">Represents a custom mail tip.</span></span>  <br/> |
|<span data-ttu-id="1dc27-129">екстерналмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="1dc27-129">ExternalMemberCount</span></span>  <br/> |<span data-ttu-id="1dc27-130">Представляет количество внешних элементов.</span><span class="sxs-lookup"><span data-stu-id="1dc27-130">Represents the count of external members.</span></span>  <br/> |
|<span data-ttu-id="1dc27-131">тоталмемберкаунт</span><span class="sxs-lookup"><span data-stu-id="1dc27-131">TotalMemberCount</span></span>  <br/> |<span data-ttu-id="1dc27-132">Представляет количество всех элементов.</span><span class="sxs-lookup"><span data-stu-id="1dc27-132">Represents the count of all members.</span></span>  <br/> |
|<span data-ttu-id="1dc27-133">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="1dc27-133">MaxMessageSize</span></span>  <br/> |<span data-ttu-id="1dc27-134">Представляет максимальный размер сообщения, которое может принимать получатель.</span><span class="sxs-lookup"><span data-stu-id="1dc27-134">Represents the maximum message size a recipient can accept.</span></span>  <br/> |
|<span data-ttu-id="1dc27-135">деливерирестриктион</span><span class="sxs-lookup"><span data-stu-id="1dc27-135">DeliveryRestriction</span></span>  <br/> |<span data-ttu-id="1dc27-136">Указывает, будут ли ограничения доставки допустить достижение получателю сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="1dc27-136">Indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span>  <br/> |
|<span data-ttu-id="1dc27-137">модератионстатус</span><span class="sxs-lookup"><span data-stu-id="1dc27-137">ModerationStatus</span></span>  <br/> |<span data-ttu-id="1dc27-138">Указывает, будет ли сообщение отправителя проверено модератором.</span><span class="sxs-lookup"><span data-stu-id="1dc27-138">Indicates whether the sender's message will be reviewed by a moderator.</span></span>  <br/> |
|<span data-ttu-id="1dc27-139">инвалидреЦипиент</span><span class="sxs-lookup"><span data-stu-id="1dc27-139">InvalidRecipient</span></span>  <br/> |<span data-ttu-id="1dc27-140">Указывает, является ли получатель недопустимым.</span><span class="sxs-lookup"><span data-stu-id="1dc27-140">Indicates whether the recipient is invalid.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1dc27-141">Примечания</span><span class="sxs-lookup"><span data-stu-id="1dc27-141">Remarks</span></span>

<span data-ttu-id="1dc27-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dc27-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dc27-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1dc27-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dc27-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1dc27-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dc27-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1dc27-145">Schema Name</span></span>  <br/> |<span data-ttu-id="1dc27-146">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1dc27-146">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dc27-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1dc27-147">Validation File</span></span>  <br/> |<span data-ttu-id="1dc27-148">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1dc27-148">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dc27-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1dc27-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dc27-150">False</span><span class="sxs-lookup"><span data-stu-id="1dc27-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dc27-151">См. также</span><span class="sxs-lookup"><span data-stu-id="1dc27-151">See also</span></span>



- [<span data-ttu-id="1dc27-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1dc27-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

