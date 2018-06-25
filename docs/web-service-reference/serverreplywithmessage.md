---
title: ServerReplyWithMessage
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
description: Элемент ServerReplyWithMessage указывает идентификатор шаблона сообщения, которые отправляются в виде ответа на входящие сообщения.
ms.openlocfilehash: f2d927ae18ac68523d4cdd173f0474fbbeb36c98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835390"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="667c6-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="667c6-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="667c6-104">Элемент **ServerReplyWithMessage** указывает идентификатор шаблона сообщения, которые отправляются в виде ответа на входящие сообщения.</span><span class="sxs-lookup"><span data-stu-id="667c6-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="667c6-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="667c6-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="667c6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="667c6-106">Attributes and elements</span></span>

<span data-ttu-id="667c6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="667c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="667c6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="667c6-108">Attributes</span></span>

<span data-ttu-id="667c6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="667c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="667c6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="667c6-110">Child elements</span></span>

|<span data-ttu-id="667c6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="667c6-111">**Element**</span></span>|<span data-ttu-id="667c6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="667c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="667c6-113">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="667c6-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="667c6-114">Представляет уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="667c6-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="667c6-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="667c6-115">Parent elements</span></span>

|<span data-ttu-id="667c6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="667c6-116">**Element**</span></span>|<span data-ttu-id="667c6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="667c6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="667c6-118">Действия</span><span class="sxs-lookup"><span data-stu-id="667c6-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="667c6-119">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="667c6-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="667c6-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="667c6-120">Text value</span></span>

<span data-ttu-id="667c6-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="667c6-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="667c6-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="667c6-122">Remarks</span></span>

<span data-ttu-id="667c6-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="667c6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="667c6-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="667c6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="667c6-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="667c6-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="667c6-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="667c6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="667c6-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="667c6-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="667c6-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="667c6-128">Validation File</span></span>  <br/> |<span data-ttu-id="667c6-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="667c6-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="667c6-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="667c6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="667c6-131">True</span><span class="sxs-lookup"><span data-stu-id="667c6-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="667c6-132">См. также</span><span class="sxs-lookup"><span data-stu-id="667c6-132">See also</span></span>



- [<span data-ttu-id="667c6-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="667c6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

