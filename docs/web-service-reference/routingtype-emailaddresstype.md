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
ms.openlocfilehash: d4229f2857a5c99cc9bb7ff9b9b103de099a0055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465088"
---
# <a name="routingtype-emailaddresstype"></a><span data-ttu-id="ae572-103">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ae572-103">RoutingType (EmailAddressType)</span></span>

<span data-ttu-id="ae572-104">Элемент **раутингтипе** определяет тип адреса для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="ae572-104">The **RoutingType** element defines the address type for the mailbox.</span></span> 
  
```XML
<RoutingType/>
```

 <span data-ttu-id="ae572-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="ae572-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ae572-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ae572-106">Attributes and elements</span></span>

<span data-ttu-id="ae572-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ae572-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae572-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ae572-108">Attributes</span></span>

<span data-ttu-id="ae572-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae572-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae572-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ae572-110">Child elements</span></span>

<span data-ttu-id="ae572-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ae572-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae572-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ae572-112">Parent elements</span></span>

|<span data-ttu-id="ae572-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ae572-113">**Element**</span></span>|<span data-ttu-id="ae572-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ae572-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae572-115">актингас</span><span class="sxs-lookup"><span data-stu-id="ae572-115">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="ae572-116">Указывает, кому отправляется вызывающий абонент.</span><span class="sxs-lookup"><span data-stu-id="ae572-116">Identifies who the caller is sending as.</span></span>  <br/> |
|[<span data-ttu-id="ae572-117">Mailbox</span><span class="sxs-lookup"><span data-stu-id="ae572-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ae572-118">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ae572-118">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="ae572-119">RoomList</span><span class="sxs-lookup"><span data-stu-id="ae572-119">RoomList</span></span>](roomlist.md) <br/> |<span data-ttu-id="ae572-120">Определяет список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="ae572-120">Identifies a list of meeting rooms.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae572-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ae572-121">Text value</span></span>

<span data-ttu-id="ae572-122">Текстовое значение представляет тип маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="ae572-122">The text value represents a routing type.</span></span> <span data-ttu-id="ae572-123">SMTP — это обычное текстовое значение для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ae572-123">SMTP is the typical text value for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae572-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="ae572-124">Remarks</span></span>

<span data-ttu-id="ae572-125">Этот элемент является необязательным для элемента [Mailbox](mailbox.md) .</span><span class="sxs-lookup"><span data-stu-id="ae572-125">This element is optional in the [Mailbox](mailbox.md) element.</span></span> <span data-ttu-id="ae572-126">Для операций доступности используется другой элемент [раутингтипе (EmailAddress)](routingtype-emailaddress.md) .</span><span class="sxs-lookup"><span data-stu-id="ae572-126">Another [RoutingType (EmailAddress)](routingtype-emailaddress.md) element is used for Availability operations.</span></span> 
  
<span data-ttu-id="ae572-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ae572-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae572-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ae572-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae572-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ae572-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae572-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ae572-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ae572-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ae572-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae572-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ae572-132">Validation File</span></span>  <br/> |<span data-ttu-id="ae572-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ae572-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae572-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ae572-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae572-135">False</span><span class="sxs-lookup"><span data-stu-id="ae572-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae572-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ae572-136">See also</span></span>



- [<span data-ttu-id="ae572-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ae572-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

