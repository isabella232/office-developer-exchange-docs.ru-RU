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
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835252"
---
# <a name="roomlists"></a><span data-ttu-id="523b3-103">румлистс</span><span class="sxs-lookup"><span data-stu-id="523b3-103">RoomLists</span></span>

<span data-ttu-id="523b3-104">Элемент **румлистс** — это список из одного или нескольких адресов, которые представляют список комнат для собраний.</span><span class="sxs-lookup"><span data-stu-id="523b3-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="523b3-105">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="523b3-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="523b3-106">румлистс</span><span class="sxs-lookup"><span data-stu-id="523b3-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="523b3-107">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="523b3-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="523b3-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="523b3-108">Attributes and elements</span></span>

<span data-ttu-id="523b3-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="523b3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="523b3-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="523b3-110">Attributes</span></span>

<span data-ttu-id="523b3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="523b3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="523b3-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="523b3-112">Child elements</span></span>

|<span data-ttu-id="523b3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="523b3-113">**Element**</span></span>|<span data-ttu-id="523b3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="523b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="523b3-115">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="523b3-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="523b3-116">Определяет адрес электронной почты и отображаемое имя, представляющее список помещений.</span><span class="sxs-lookup"><span data-stu-id="523b3-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="523b3-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="523b3-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="523b3-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="523b3-118">Parent elements</span></span>

|<span data-ttu-id="523b3-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="523b3-119">**Element**</span></span>|<span data-ttu-id="523b3-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="523b3-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="523b3-121">жетрумлистсреспонсе</span><span class="sxs-lookup"><span data-stu-id="523b3-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="523b3-122">Содержит состояние и результат запроса [операции GetRoomLists](getroomlists-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="523b3-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="523b3-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="523b3-123">Remarks</span></span>

<span data-ttu-id="523b3-124">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="523b3-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="523b3-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="523b3-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="523b3-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="523b3-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="523b3-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="523b3-127">Schema Name</span></span>  <br/> |<span data-ttu-id="523b3-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="523b3-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="523b3-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="523b3-129">Validation File</span></span>  <br/> |<span data-ttu-id="523b3-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="523b3-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="523b3-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="523b3-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="523b3-132">False</span><span class="sxs-lookup"><span data-stu-id="523b3-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="523b3-133">См. также</span><span class="sxs-lookup"><span data-stu-id="523b3-133">See also</span></span>



[<span data-ttu-id="523b3-134">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="523b3-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="523b3-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="523b3-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

