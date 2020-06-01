---
title: румлистс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: Элемент Румлистс — это список из одного или нескольких адресов, которые представляют список комнат для собраний.
ms.openlocfilehash: 8f6393b617331e5878e48113c94ca3546cba095e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459050"
---
# <a name="roomlists"></a><span data-ttu-id="bfbef-103">румлистс</span><span class="sxs-lookup"><span data-stu-id="bfbef-103">RoomLists</span></span>

<span data-ttu-id="bfbef-104">Элемент **румлистс** — это список из одного или нескольких адресов, которые представляют список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="bfbef-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="bfbef-105">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="bfbef-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="bfbef-106">румлистс</span><span class="sxs-lookup"><span data-stu-id="bfbef-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="bfbef-107">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="bfbef-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bfbef-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bfbef-108">Attributes and elements</span></span>

<span data-ttu-id="bfbef-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bfbef-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bfbef-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bfbef-110">Attributes</span></span>

<span data-ttu-id="bfbef-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bfbef-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bfbef-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bfbef-112">Child elements</span></span>

|<span data-ttu-id="bfbef-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bfbef-113">**Element**</span></span>|<span data-ttu-id="bfbef-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bfbef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfbef-115">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="bfbef-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="bfbef-116">Определяет адрес электронной почты и отображаемое имя, представляющее список помещений.</span><span class="sxs-lookup"><span data-stu-id="bfbef-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="bfbef-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bfbef-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bfbef-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bfbef-118">Parent elements</span></span>

|<span data-ttu-id="bfbef-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bfbef-119">**Element**</span></span>|<span data-ttu-id="bfbef-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bfbef-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bfbef-121">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="bfbef-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="bfbef-122">Содержит состояние и результат запроса [операции GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bfbef-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bfbef-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="bfbef-123">Remarks</span></span>

<span data-ttu-id="bfbef-124">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bfbef-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bfbef-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bfbef-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bfbef-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bfbef-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bfbef-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bfbef-127">Schema Name</span></span>  <br/> |<span data-ttu-id="bfbef-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bfbef-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bfbef-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bfbef-129">Validation File</span></span>  <br/> |<span data-ttu-id="bfbef-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bfbef-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bfbef-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bfbef-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="bfbef-132">False</span><span class="sxs-lookup"><span data-stu-id="bfbef-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bfbef-133">См. также</span><span class="sxs-lookup"><span data-stu-id="bfbef-133">See also</span></span>



[<span data-ttu-id="bfbef-134">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="bfbef-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="bfbef-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bfbef-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

