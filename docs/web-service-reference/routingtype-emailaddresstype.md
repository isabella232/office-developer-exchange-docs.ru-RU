---
title: RoutingType (EmailAddressType)
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
description: Элемент RoutingType определяет тип адреса для почтового ящика.
ms.openlocfilehash: a02c3b5711a657311428d67cccabd9c8c231db67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835256"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="b07fa-103">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b07fa-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="b07fa-104">Элемент **RoutingType** определяет тип адреса для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b07fa-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="b07fa-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="b07fa-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b07fa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b07fa-106">Attributes and elements</span></span>

<span data-ttu-id="b07fa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b07fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b07fa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b07fa-108">Attributes</span></span>

<span data-ttu-id="b07fa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b07fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b07fa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b07fa-110">Child elements</span></span>

<span data-ttu-id="b07fa-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b07fa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b07fa-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b07fa-112">Parent elements</span></span>

|<span data-ttu-id="b07fa-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b07fa-113">**Element**</span></span>|<span data-ttu-id="b07fa-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b07fa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b07fa-115">ActingAs</span><span class="sxs-lookup"><span data-stu-id="b07fa-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="b07fa-116">Определяет, как отправляющего вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="b07fa-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="b07fa-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="b07fa-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="b07fa-118">Определяет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="b07fa-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="b07fa-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="b07fa-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="b07fa-120">Определяет список конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="b07fa-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b07fa-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b07fa-121">Text value</span></span>

<span data-ttu-id="b07fa-122">Текстовое значение представляет тип маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="b07fa-122">The text value represents a routing type.</span></span> <span data-ttu-id="b07fa-123">SMTP — типичное текстовое значение для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b07fa-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b07fa-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="b07fa-124">Remarks</span></span>

<span data-ttu-id="b07fa-125">Этот элемент является необязательным в элементе [почтового ящика](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="b07fa-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="b07fa-126">Другой элемент [RoutingType (EmailAddress)](routingtype-emailaddress.md) используется для операций доступности.</span><span class="sxs-lookup"><span data-stu-id="b07fa-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="b07fa-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b07fa-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b07fa-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b07fa-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b07fa-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b07fa-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b07fa-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b07fa-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b07fa-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b07fa-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b07fa-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b07fa-132">Validation File</span></span>  <br/> |<span data-ttu-id="b07fa-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b07fa-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b07fa-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b07fa-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b07fa-135">False</span><span class="sxs-lookup"><span data-stu-id="b07fa-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b07fa-136">См. также</span><span class="sxs-lookup"><span data-stu-id="b07fa-136">See also</span></span>



- [<span data-ttu-id="b07fa-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b07fa-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

