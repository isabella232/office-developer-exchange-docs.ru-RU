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
description: Элемент RoomList принимают одиночные представляет адрес электронной почты, который определяет список комнат для собраний.
ms.openlocfilehash: 0444475cb9fffbb89ba2861096baee0c7e645995
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460521"
---
# <a name="roomlist"></a><span data-ttu-id="171f1-103">RoomList</span><span class="sxs-lookup"><span data-stu-id="171f1-103">RoomList</span></span>

<span data-ttu-id="171f1-104">Элемент **RoomList принимают одиночные** представляет адрес электронной почты, который определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="171f1-104">The **RoomList** element represents an e-mail address that identifies a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="171f1-105">GetRooms</span><span class="sxs-lookup"><span data-stu-id="171f1-105">GetRooms</span></span>](getrooms.md)
  
[<span data-ttu-id="171f1-106">RoomList</span><span class="sxs-lookup"><span data-stu-id="171f1-106">RoomList</span></span>](roomlist.md)
  
```XML
<RoomList>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RoomList>
```

 <span data-ttu-id="171f1-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="171f1-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="171f1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="171f1-108">Attributes and elements</span></span>

<span data-ttu-id="171f1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="171f1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="171f1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="171f1-110">Attributes</span></span>

<span data-ttu-id="171f1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="171f1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="171f1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="171f1-112">Child elements</span></span>

|<span data-ttu-id="171f1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="171f1-113">**Element**</span></span>|<span data-ttu-id="171f1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="171f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="171f1-115">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="171f1-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="171f1-116">Определяет отображаемое имя списка помещений.</span><span class="sxs-lookup"><span data-stu-id="171f1-116">Defines the display name of the room list.</span></span> <span data-ttu-id="171f1-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="171f1-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="171f1-118">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="171f1-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="171f1-119">Определяет SMTP-адрес списка помещений.</span><span class="sxs-lookup"><span data-stu-id="171f1-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a room list.</span></span> <span data-ttu-id="171f1-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="171f1-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="171f1-121">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="171f1-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="171f1-122">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="171f1-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="171f1-123">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="171f1-123">The default is SMTP.</span></span> <span data-ttu-id="171f1-124">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="171f1-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="171f1-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="171f1-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="171f1-126">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="171f1-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="171f1-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="171f1-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="171f1-128">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="171f1-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="171f1-129">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="171f1-129">Defines the item identifier of a contact or private distribution list for recipients from a user's Contacts folder.</span></span> <span data-ttu-id="171f1-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="171f1-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="171f1-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="171f1-131">Parent elements</span></span>

|<span data-ttu-id="171f1-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="171f1-132">**Element**</span></span>|<span data-ttu-id="171f1-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="171f1-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="171f1-134">GetRooms</span><span class="sxs-lookup"><span data-stu-id="171f1-134">GetRooms</span></span>](getrooms.md) <br/> |<span data-ttu-id="171f1-135">Корневой элемент запроса для получения списка комнат в определенном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="171f1-135">The root element in a request to get a list of rooms within a particular room list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="171f1-136">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="171f1-136">Text value</span></span>

<span data-ttu-id="171f1-137">Нет.</span><span class="sxs-lookup"><span data-stu-id="171f1-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="171f1-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="171f1-138">Remarks</span></span>

<span data-ttu-id="171f1-139">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="171f1-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="171f1-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="171f1-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="171f1-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="171f1-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="171f1-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="171f1-142">Schema Name</span></span>  <br/> |<span data-ttu-id="171f1-143">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="171f1-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="171f1-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="171f1-144">Validation File</span></span>  <br/> |<span data-ttu-id="171f1-145">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="171f1-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="171f1-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="171f1-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="171f1-147">False</span><span class="sxs-lookup"><span data-stu-id="171f1-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="171f1-148">См. также</span><span class="sxs-lookup"><span data-stu-id="171f1-148">See also</span></span>



[<span data-ttu-id="171f1-149">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="171f1-149">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="171f1-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="171f1-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

