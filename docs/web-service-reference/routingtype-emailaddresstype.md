---
title: Раутингтипе (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 683216be-9972-4f48-a148-c34bfe7f53e5
description: Элемент Раутингтипе определяет тип адреса для почтового ящика.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="b5b8e-103">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b5b8e-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="b5b8e-104">Элемент **раутингтипе** определяет тип адреса для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="b5b8e-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="b5b8e-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5b8e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5b8e-106">Attributes and elements</span></span>

<span data-ttu-id="b5b8e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5b8e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5b8e-108">Attributes</span></span>

<span data-ttu-id="b5b8e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b5b8e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5b8e-110">Child elements</span></span>

<span data-ttu-id="b5b8e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5b8e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5b8e-112">Parent elements</span></span>

|<span data-ttu-id="b5b8e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b5b8e-113">**Element**</span></span>|<span data-ttu-id="b5b8e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5b8e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5b8e-115">актингас</span><span class="sxs-lookup"><span data-stu-id="b5b8e-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="b5b8e-116">Указывает, кому отправляется вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="b5b8e-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="b5b8e-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b5b8e-118">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="b5b8e-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="b5b8e-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="b5b8e-120">Определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5b8e-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b5b8e-121">Text value</span></span>

<span data-ttu-id="b5b8e-122">Текстовое значение представляет тип маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-122">The text value represents a routing type.</span></span> <span data-ttu-id="b5b8e-123">SMTP — это обычное текстовое значение для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5b8e-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="b5b8e-124">Remarks</span></span>

<span data-ttu-id="b5b8e-125">Этот элемент является необязательным для элемента [Mailbox](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="b5b8e-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="b5b8e-126">Для операций доступности используется другой элемент [раутингтипе (EmailAddress)](routingtype-emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="b5b8e-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="b5b8e-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b5b8e-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5b8e-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b5b8e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5b8e-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b5b8e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5b8e-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b5b8e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b5b8e-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b5b8e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5b8e-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b5b8e-132">Validation File</span></span>  <br/> |<span data-ttu-id="b5b8e-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5b8e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5b8e-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b5b8e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5b8e-135">False</span><span class="sxs-lookup"><span data-stu-id="b5b8e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5b8e-136">См. также</span><span class="sxs-lookup"><span data-stu-id="b5b8e-136">See also</span></span>



- [<span data-ttu-id="b5b8e-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b5b8e-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

