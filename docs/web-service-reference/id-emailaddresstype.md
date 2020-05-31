---
title: ID (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 3e1e37b5-5469-4447-ad1f-c2c6d4e0482f
description: Элемент ID определяет комнату для собраний в организации Exchange Server.
ms.openlocfilehash: 5cd62f6f4e5912d2ecccda352be15c6a3b24e06c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833847"
---
# <a name="id-emailaddresstype"></a><span data-ttu-id="a2f67-103">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a2f67-103">Id (EmailAddressType)</span></span>

<span data-ttu-id="a2f67-104">Элемент **ID** определяет комнату для собраний в организации Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a2f67-104">The **Id** element identifies a meeting room within the Exchange server organization.</span></span> 
  
[<span data-ttu-id="a2f67-105">Комната</span><span class="sxs-lookup"><span data-stu-id="a2f67-105">Room</span></span>](room.md)
  
[<span data-ttu-id="a2f67-106">ID (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a2f67-106">Id (EmailAddressType)</span></span>](id-emailaddresstype.md)
  
```xml
<Id>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Id>
```

 <span data-ttu-id="a2f67-107">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="a2f67-107">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2f67-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2f67-108">Attributes and elements</span></span>

<span data-ttu-id="a2f67-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a2f67-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2f67-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2f67-110">Attributes</span></span>

<span data-ttu-id="a2f67-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a2f67-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2f67-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2f67-112">Child elements</span></span>

|<span data-ttu-id="a2f67-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2f67-113">**Element**</span></span>|<span data-ttu-id="a2f67-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2f67-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2f67-115">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a2f67-115">Name (EmailAddressType)</span></span>](name-emailaddresstype.md) <br/> |<span data-ttu-id="a2f67-116">Определяет имя комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="a2f67-116">Defines the name of the meeting room.</span></span> <span data-ttu-id="a2f67-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a2f67-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a2f67-118">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="a2f67-118">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="a2f67-119">Определяет SMTP-адрес комнаты для собраний.</span><span class="sxs-lookup"><span data-stu-id="a2f67-119">Defines the Simple Mail Transfer Protocol (SMTP) address of a meeting room.</span></span> <span data-ttu-id="a2f67-120">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a2f67-120">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a2f67-121">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a2f67-121">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="a2f67-122">Определяет маршрутизацию, используемую для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a2f67-122">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="a2f67-123">По умолчанию используется протокол SMTP.</span><span class="sxs-lookup"><span data-stu-id="a2f67-123">The default is SMTP.</span></span> <span data-ttu-id="a2f67-124">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a2f67-124">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a2f67-125">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a2f67-125">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="a2f67-126">Определяет тип почтового ящика пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a2f67-126">Defines the mailbox type of a mailbox user.</span></span> <span data-ttu-id="a2f67-127">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a2f67-127">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a2f67-128">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a2f67-128">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a2f67-129">Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2f67-129">Defines the item identifier of a contact or private distribution list for recipients from a user's contacts folder.</span></span> <span data-ttu-id="a2f67-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a2f67-130">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2f67-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2f67-131">Parent elements</span></span>

|<span data-ttu-id="a2f67-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2f67-132">**Element**</span></span>|<span data-ttu-id="a2f67-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2f67-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2f67-134">Комната</span><span class="sxs-lookup"><span data-stu-id="a2f67-134">Room</span></span>](room.md) <br/> |<span data-ttu-id="a2f67-135">Определяет комнату для собраний в организации Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a2f67-135">Defines a meeting room in the Exchange server organization.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2f67-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="a2f67-136">Remarks</span></span>

<span data-ttu-id="a2f67-137">Схема, описывающая этот элемент, находится в каталоге EWS компьютера под управлением Microsoft Exchange Server, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2f67-137">The schema that describes this element is located in the EWS directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2f67-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a2f67-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2f67-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a2f67-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2f67-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a2f67-140">Schema Name</span></span>  <br/> |<span data-ttu-id="a2f67-141">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a2f67-141">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2f67-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a2f67-142">Validation File</span></span>  <br/> |<span data-ttu-id="a2f67-143">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a2f67-143">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2f67-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a2f67-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="a2f67-145">False</span><span class="sxs-lookup"><span data-stu-id="a2f67-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2f67-146">См. также</span><span class="sxs-lookup"><span data-stu-id="a2f67-146">See also</span></span>



[<span data-ttu-id="a2f67-147">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="a2f67-147">GetRooms operation</span></span>](getrooms-operation.md)


- [<span data-ttu-id="a2f67-148">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2f67-148">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

