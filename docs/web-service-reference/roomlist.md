---
title: RoomList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomList
api_type:
- schema
ms.assetid: cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2
description: Элемент RoomList представляет адрес электронной почты, который определяет список конференц-залы.
ms.openlocfilehash: 7de2c67f8001387abf463186933f0b81ee45a58a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835262"
---
# <a name="roomlist"></a><span data-ttu-id="87f06-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="87f06-103">RoomList</span></span>

<span data-ttu-id="87f06-104">Элемент **RoomList** представляет адрес электронной почты, который определяет список конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="87f06-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="87f06-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="87f06-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="87f06-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="87f06-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="87f06-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="87f06-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87f06-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="87f06-108">Attributes and elements</span></span>

<span data-ttu-id="87f06-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="87f06-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87f06-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="87f06-110">Attributes</span></span>

<span data-ttu-id="87f06-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="87f06-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87f06-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="87f06-112">Child elements</span></span>

|<span data-ttu-id="87f06-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87f06-113">**Element**</span></span>|<span data-ttu-id="87f06-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87f06-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87f06-115">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="87f06-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="87f06-116">Задает отображаемое имя список помещений.</span><span class="sxs-lookup"><span data-stu-id="87f06-116">Defines the display name of the room list.</span></span> <span data-ttu-id="87f06-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="87f06-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="87f06-118">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="87f06-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="87f06-119">Определяет адрес Simple Mail Transfer Protocol (SMTP) в список помещений.</span><span class="sxs-lookup"><span data-stu-id="87f06-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="87f06-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="87f06-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="87f06-121">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="87f06-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="87f06-122">Определяет маршрутизации, используемый для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="87f06-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="87f06-123">Значение по умолчанию — SMTP.</span><span class="sxs-lookup"><span data-stu-id="87f06-123">The default is SMTP.</span></span> <span data-ttu-id="87f06-124">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="87f06-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="87f06-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="87f06-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="87f06-126">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="87f06-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="87f06-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="87f06-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="87f06-128">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="87f06-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="87f06-129">Определяет идентификатор элемента контакта или список рассылки закрытый для получателей из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="87f06-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="87f06-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="87f06-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87f06-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="87f06-131">Parent elements</span></span>

|<span data-ttu-id="87f06-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="87f06-132">**Element**</span></span>|<span data-ttu-id="87f06-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="87f06-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87f06-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="87f06-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="87f06-135">Корневой элемент в запросе для получения списка комнат в пределах определенного почтового ящика помещения.</span><span class="sxs-lookup"><span data-stu-id="87f06-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="87f06-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="87f06-136">Text value</span></span>

<span data-ttu-id="87f06-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="87f06-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="87f06-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="87f06-138">Remarks</span></span>

<span data-ttu-id="87f06-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="87f06-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87f06-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="87f06-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87f06-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="87f06-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87f06-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="87f06-142">Schema Name</span></span>  <br/> |<span data-ttu-id="87f06-143">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="87f06-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87f06-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="87f06-144">Validation File</span></span>  <br/> |<span data-ttu-id="87f06-145">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="87f06-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87f06-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="87f06-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="87f06-147">False</span><span class="sxs-lookup"><span data-stu-id="87f06-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87f06-148">См. также</span><span class="sxs-lookup"><span data-stu-id="87f06-148">See also</span></span>



[<span data-ttu-id="87f06-149">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="87f06-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="87f06-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="87f06-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

