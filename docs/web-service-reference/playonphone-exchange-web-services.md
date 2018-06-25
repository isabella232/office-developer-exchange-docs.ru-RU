---
title: PlayOnPhone (веб-служб Exchange)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 486612be-470c-4f99-929a-f2b283e055c1
description: Элемент PlayOnPhone представляет запрос на его чтение на телефоне.
ms.openlocfilehash: 75493a31940ea609fd6cf454e91ca5881fb7e678
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834816"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="5337c-103">PlayOnPhone (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="5337c-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="5337c-104">Элемент **PlayOnPhone** представляет запрос на его чтение на телефоне.</span><span class="sxs-lookup"><span data-stu-id="5337c-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="5337c-105">**PlayOnPhoneType**</span><span class="sxs-lookup"><span data-stu-id="5337c-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5337c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5337c-106">Attributes and elements</span></span>

<span data-ttu-id="5337c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5337c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5337c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5337c-108">Attributes</span></span>

<span data-ttu-id="5337c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5337c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5337c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5337c-110">Child elements</span></span>

|<span data-ttu-id="5337c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5337c-111">**Element**</span></span>|<span data-ttu-id="5337c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5337c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5337c-113">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5337c-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5337c-114">Представляет идентификатор элемента для воспроизведения на телефоне.</span><span class="sxs-lookup"><span data-stu-id="5337c-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="5337c-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="5337c-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="5337c-116">DialString (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="5337c-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="5337c-117">Представляет строку телефонные номера телефона, который вызывается для воспроизведения элемента по телефону.</span><span class="sxs-lookup"><span data-stu-id="5337c-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="5337c-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="5337c-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5337c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5337c-119">Parent elements</span></span>

<span data-ttu-id="5337c-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="5337c-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5337c-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="5337c-121">Remarks</span></span>

<span data-ttu-id="5337c-122">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5337c-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5337c-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5337c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5337c-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5337c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5337c-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5337c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="5337c-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5337c-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5337c-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5337c-127">Validation File</span></span>  <br/> |<span data-ttu-id="5337c-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5337c-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5337c-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5337c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="5337c-130">False</span><span class="sxs-lookup"><span data-stu-id="5337c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5337c-131">См. также</span><span class="sxs-lookup"><span data-stu-id="5337c-131">See also</span></span>



- [<span data-ttu-id="5337c-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5337c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

