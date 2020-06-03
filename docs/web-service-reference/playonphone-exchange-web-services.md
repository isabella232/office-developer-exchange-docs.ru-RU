---
title: PlayOnPhone (веб-службы Exchange)
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
description: Элемент PlayOnPhone представляет запрос на чтение элемента на телефоне.
ms.openlocfilehash: e2c09a67255106ad9afddb86fa19b7a4a5762ee5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466250"
---
# <a name="playonphone-exchange-web-services"></a><span data-ttu-id="fbde1-103">PlayOnPhone (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="fbde1-103">PlayOnPhone (Exchange Web Services)</span></span>

<span data-ttu-id="fbde1-104">Элемент **PlayOnPhone** представляет запрос на чтение элемента на телефоне.</span><span class="sxs-lookup"><span data-stu-id="fbde1-104">The **PlayOnPhone** element represents a request to read an item on a phone.</span></span> 
  
```xml
<PlayOnPhone>   <ItemId/>   <DialString/></PlayOnPhone>
```

 <span data-ttu-id="fbde1-105">**плайонфонетипе**</span><span class="sxs-lookup"><span data-stu-id="fbde1-105">**PlayOnPhoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fbde1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fbde1-106">Attributes and elements</span></span>

<span data-ttu-id="fbde1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fbde1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbde1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fbde1-108">Attributes</span></span>

<span data-ttu-id="fbde1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fbde1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbde1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fbde1-110">Child elements</span></span>

|<span data-ttu-id="fbde1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fbde1-111">**Element**</span></span>|<span data-ttu-id="fbde1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fbde1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbde1-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="fbde1-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="fbde1-114">Представляет идентификатор элемента, который будет воспроизводиться на телефоне.</span><span class="sxs-lookup"><span data-stu-id="fbde1-114">Represents the identifier of an item to play on a phone.</span></span> <span data-ttu-id="fbde1-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbde1-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="fbde1-116">DialString (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="fbde1-116">DialString (Exchange Web Services)</span></span>](dialstring-exchange-web-services.md) <br/> |<span data-ttu-id="fbde1-117">Представляет строку набора номера телефона, который вызывается для проигрывания элемента по телефону.</span><span class="sxs-lookup"><span data-stu-id="fbde1-117">Represents the dial string of the phone number that is called to play an item by phone.</span></span> <span data-ttu-id="fbde1-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="fbde1-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fbde1-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fbde1-119">Parent elements</span></span>

<span data-ttu-id="fbde1-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="fbde1-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fbde1-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="fbde1-121">Remarks</span></span>

<span data-ttu-id="fbde1-122">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fbde1-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fbde1-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fbde1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fbde1-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fbde1-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fbde1-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fbde1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fbde1-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fbde1-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fbde1-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fbde1-127">Validation File</span></span>  <br/> |<span data-ttu-id="fbde1-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fbde1-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fbde1-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fbde1-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fbde1-130">False</span><span class="sxs-lookup"><span data-stu-id="fbde1-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fbde1-131">См. также</span><span class="sxs-lookup"><span data-stu-id="fbde1-131">See also</span></span>



- [<span data-ttu-id="fbde1-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fbde1-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

