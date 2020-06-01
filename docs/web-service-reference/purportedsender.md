---
title: пурпортедсендер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PurportedSender
api_type:
- schema
ms.assetid: eb7a54ec-2e48-4030-bbcf-50a31609691b
description: Элемент Пурпортедсендер содержит контактные данные отправителя предполагаемым сообщения электронной почты.
ms.openlocfilehash: 5ecf352484a423e3955736620bf5a65c4e98099a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468336"
---
# <a name="purportedsender"></a><span data-ttu-id="cd13f-103">пурпортедсендер</span><span class="sxs-lookup"><span data-stu-id="cd13f-103">PurportedSender</span></span>

<span data-ttu-id="cd13f-104">Элемент **пурпортедсендер** содержит контактные данные отправителя предполагаемым сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cd13f-104">The **PurportedSender** element contains contact information for the alleged sender of an e-mail message.</span></span> 
  
```XML
<PurportedSender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</PurportedSender>
```

 <span data-ttu-id="cd13f-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="cd13f-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd13f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cd13f-106">Attributes and elements</span></span>

<span data-ttu-id="cd13f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cd13f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd13f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cd13f-108">Attributes</span></span>

<span data-ttu-id="cd13f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cd13f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd13f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cd13f-110">Child elements</span></span>

|<span data-ttu-id="cd13f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd13f-111">**Element**</span></span>|<span data-ttu-id="cd13f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd13f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd13f-113">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="cd13f-113">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="cd13f-114">Представляет имя пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="cd13f-114">Represents the name of the mailbox user.</span></span> <span data-ttu-id="cd13f-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd13f-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cd13f-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="cd13f-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="cd13f-117">Определяет SMTP-адрес пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="cd13f-117">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="cd13f-118">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd13f-118">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cd13f-119">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="cd13f-119">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="cd13f-120">Представляет протокол маршрутизации для получателя.</span><span class="sxs-lookup"><span data-stu-id="cd13f-120">Represents the routing protocol for the recipient.</span></span> <span data-ttu-id="cd13f-121">По умолчанию используется значение SMTP.</span><span class="sxs-lookup"><span data-stu-id="cd13f-121">The default value is SMTP.</span></span> <span data-ttu-id="cd13f-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd13f-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cd13f-123">MailboxType</span><span class="sxs-lookup"><span data-stu-id="cd13f-123">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="cd13f-124">Представляет тип почтового ящика, представленного адресом электронной почты..</span><span class="sxs-lookup"><span data-stu-id="cd13f-124">Represents the type of mailbox that is represented by the e-mail address..</span></span> <span data-ttu-id="cd13f-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd13f-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="cd13f-126">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="cd13f-126">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="cd13f-127">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="cd13f-127">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="cd13f-128">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd13f-128">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd13f-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cd13f-129">Parent elements</span></span>

|<span data-ttu-id="cd13f-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd13f-130">**Element**</span></span>|<span data-ttu-id="cd13f-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd13f-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd13f-132">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cd13f-132">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="cd13f-133">Задает условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="cd13f-133">Specifies criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="cd13f-134">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cd13f-134">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="cd13f-135">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cd13f-135">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="cd13f-136">мессажетраккингсеарчресулт</span><span class="sxs-lookup"><span data-stu-id="cd13f-136">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="cd13f-137">Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="cd13f-137">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd13f-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cd13f-138">Text value</span></span>

<span data-ttu-id="cd13f-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="cd13f-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd13f-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="cd13f-140">Remarks</span></span>

<span data-ttu-id="cd13f-141">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd13f-141">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd13f-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cd13f-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd13f-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cd13f-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cd13f-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cd13f-144">Schema Name</span></span>  <br/> |<span data-ttu-id="cd13f-145">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cd13f-145">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cd13f-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cd13f-146">Validation File</span></span>  <br/> |<span data-ttu-id="cd13f-147">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cd13f-147">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cd13f-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cd13f-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd13f-149">False</span><span class="sxs-lookup"><span data-stu-id="cd13f-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd13f-150">См. также</span><span class="sxs-lookup"><span data-stu-id="cd13f-150">See also</span></span>



[<span data-ttu-id="cd13f-151">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="cd13f-151">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="cd13f-152">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cd13f-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

