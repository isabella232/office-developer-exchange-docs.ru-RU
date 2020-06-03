---
title: серверрепливисмессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerReplyWithMessage
api_type:
- schema
ms.assetid: 113c6ff2-9592-44f0-b542-54e4d5122ccb
description: Элемент Серверрепливисмессаже указывает идентификатор сообщения шаблона, отправляемого в качестве ответа на входящие сообщения.
ms.openlocfilehash: faaa054018a17be3ff59b9fc385b3d846d39c3f1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461977"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="68d3a-103">серверрепливисмессаже</span><span class="sxs-lookup"><span data-stu-id="68d3a-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="68d3a-104">Элемент **серверрепливисмессаже** указывает идентификатор сообщения шаблона, отправляемого в качестве ответа на входящие сообщения.</span><span class="sxs-lookup"><span data-stu-id="68d3a-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="68d3a-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="68d3a-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="68d3a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68d3a-106">Attributes and elements</span></span>

<span data-ttu-id="68d3a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="68d3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68d3a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68d3a-108">Attributes</span></span>

<span data-ttu-id="68d3a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="68d3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68d3a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68d3a-110">Child elements</span></span>

|<span data-ttu-id="68d3a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68d3a-111">**Element**</span></span>|<span data-ttu-id="68d3a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68d3a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68d3a-113">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="68d3a-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="68d3a-114">Представляет уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="68d3a-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68d3a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68d3a-115">Parent elements</span></span>

|<span data-ttu-id="68d3a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68d3a-116">**Element**</span></span>|<span data-ttu-id="68d3a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68d3a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68d3a-118">Действия</span><span class="sxs-lookup"><span data-stu-id="68d3a-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="68d3a-119">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="68d3a-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="68d3a-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="68d3a-120">Text value</span></span>

<span data-ttu-id="68d3a-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="68d3a-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68d3a-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="68d3a-122">Remarks</span></span>

<span data-ttu-id="68d3a-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="68d3a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68d3a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68d3a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68d3a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68d3a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68d3a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68d3a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="68d3a-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="68d3a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68d3a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68d3a-128">Validation File</span></span>  <br/> |<span data-ttu-id="68d3a-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="68d3a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68d3a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68d3a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="68d3a-131">True</span><span class="sxs-lookup"><span data-stu-id="68d3a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68d3a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="68d3a-132">See also</span></span>



- [<span data-ttu-id="68d3a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="68d3a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

