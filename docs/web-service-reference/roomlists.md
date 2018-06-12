---
title: RoomLists
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
description: Элемент RoomLists приведен список один или несколько адресов, которые представляют список конференц-залы.
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835252"
---
# <a name="roomlists"></a><span data-ttu-id="99594-103">RoomLists</span><span class="sxs-lookup"><span data-stu-id="99594-103">RoomLists</span></span>

<span data-ttu-id="99594-104">Элемент **RoomLists** приведен список один или несколько адресов, которые представляют список конференц-залы.</span><span class="sxs-lookup"><span data-stu-id="99594-104">The **RoomLists** element is a list of one or more addresses that represent a list of meeting rooms.</span></span> 
  
[<span data-ttu-id="99594-105">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="99594-105">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
[<span data-ttu-id="99594-106">RoomLists</span><span class="sxs-lookup"><span data-stu-id="99594-106">RoomLists</span></span>](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 <span data-ttu-id="99594-107">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="99594-107">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99594-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99594-108">Attributes and elements</span></span>

<span data-ttu-id="99594-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="99594-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99594-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99594-110">Attributes</span></span>

<span data-ttu-id="99594-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="99594-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99594-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99594-112">Child elements</span></span>

|<span data-ttu-id="99594-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99594-113">**Element**</span></span>|<span data-ttu-id="99594-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99594-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99594-115">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="99594-115">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="99594-116">Задает адрес электронной почты и отображаемое имя, представляющий список помещений.</span><span class="sxs-lookup"><span data-stu-id="99594-116">Defines the e-mail address and display name that represents the room list.</span></span> <span data-ttu-id="99594-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="99594-117">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99594-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99594-118">Parent elements</span></span>

|<span data-ttu-id="99594-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99594-119">**Element**</span></span>|<span data-ttu-id="99594-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99594-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99594-121">GetRoomListsResponse</span><span class="sxs-lookup"><span data-stu-id="99594-121">GetRoomListsResponse</span></span>](getroomlistsresponse.md) <br/> |<span data-ttu-id="99594-122">Содержит состояние и результат [операции GetRoomLists](getroomlists-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="99594-122">Contains the status and result of a [GetRoomLists operation](getroomlists-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="99594-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="99594-123">Remarks</span></span>

<span data-ttu-id="99594-124">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="99594-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99594-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99594-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99594-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99594-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="99594-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99594-127">Schema Name</span></span>  <br/> |<span data-ttu-id="99594-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="99594-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="99594-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99594-129">Validation File</span></span>  <br/> |<span data-ttu-id="99594-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="99594-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="99594-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99594-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="99594-132">False</span><span class="sxs-lookup"><span data-stu-id="99594-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99594-133">См. также</span><span class="sxs-lookup"><span data-stu-id="99594-133">See also</span></span>



[<span data-ttu-id="99594-134">Операция GetRoomLists</span><span class="sxs-lookup"><span data-stu-id="99594-134">GetRoomLists operation</span></span>](getroomlists-operation.md)


- [<span data-ttu-id="99594-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99594-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

