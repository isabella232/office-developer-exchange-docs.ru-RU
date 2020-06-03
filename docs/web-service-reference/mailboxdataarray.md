---
title: маилбоксдатааррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxDataArray
api_type:
- schema
ms.assetid: a14af788-beee-452c-b5d0-37bcb4ef02ff
description: Элемент Маилбоксдатааррай содержит список почтовых ящиков, в которых запрашиваются сведения о доступности.
ms.openlocfilehash: 894bf97a0d633d7eef0434331ccf1580fcba386e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468196"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="dad71-103">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="dad71-103">MailboxDataArray</span></span>

<span data-ttu-id="dad71-104">Элемент **маилбоксдатааррай** содержит список почтовых ящиков, в которых запрашиваются сведения о доступности.</span><span class="sxs-lookup"><span data-stu-id="dad71-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="dad71-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="dad71-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="dad71-106">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="dad71-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="dad71-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="dad71-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="dad71-108">**аррайофмаилбоксдата**</span><span class="sxs-lookup"><span data-stu-id="dad71-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dad71-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dad71-109">Attributes and elements</span></span>

<span data-ttu-id="dad71-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dad71-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dad71-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dad71-111">Attributes</span></span>

<span data-ttu-id="dad71-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dad71-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dad71-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dad71-113">Child elements</span></span>

|<span data-ttu-id="dad71-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dad71-114">**Element**</span></span>|<span data-ttu-id="dad71-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dad71-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dad71-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="dad71-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="dad71-117">Представляет отдельного пользователя почтового ящика и параметры возвращаемого типа данных об этом пользователе.</span><span class="sxs-lookup"><span data-stu-id="dad71-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dad71-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dad71-118">Parent elements</span></span>

|<span data-ttu-id="dad71-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dad71-119">**Element**</span></span>|<span data-ttu-id="dad71-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dad71-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dad71-121">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="dad71-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="dad71-122">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="dad71-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="dad71-123">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="dad71-123">This is a root element.</span></span>  <br/> <span data-ttu-id="dad71-124">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="dad71-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dad71-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="dad71-125">Remarks</span></span>

<span data-ttu-id="dad71-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dad71-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dad71-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dad71-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dad71-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dad71-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dad71-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dad71-129">Schema Name</span></span>  <br/> |<span data-ttu-id="dad71-130">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dad71-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dad71-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dad71-131">Validation File</span></span>  <br/> |<span data-ttu-id="dad71-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dad71-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dad71-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dad71-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="dad71-134">False</span><span class="sxs-lookup"><span data-stu-id="dad71-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dad71-135">См. также</span><span class="sxs-lookup"><span data-stu-id="dad71-135">See also</span></span>

- [<span data-ttu-id="dad71-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dad71-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="dad71-137">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="dad71-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="dad71-138">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="dad71-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

