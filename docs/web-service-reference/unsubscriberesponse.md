---
title: UnsubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponse
api_type:
- schema
ms.assetid: 125e0326-6522-42cd-b20e-6977e6fde249
description: Элемент UnsubscribeResponse определяет ответ на запрос отказа от подписки.
ms.openlocfilehash: a5d90a6631cba7f18da0261be52488c7f6793dcd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840306"
---
# <a name="unsubscriberesponse"></a><span data-ttu-id="607db-103">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="607db-103">UnsubscribeResponse</span></span>

<span data-ttu-id="607db-104">Элемент **UnsubscribeResponse** определяет ответ на запрос отказа от подписки.</span><span class="sxs-lookup"><span data-stu-id="607db-104">The **UnsubscribeResponse** element defines a response to an Unsubscribe request.</span></span> 
  
```xml
<UnsubscribeResponse>
   <ResponseMessages/>
</UnsubscribeResponse>
```

 <span data-ttu-id="607db-105">**UnsubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="607db-105">**UnsubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="607db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="607db-106">Attributes and elements</span></span>

<span data-ttu-id="607db-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="607db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="607db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="607db-108">Attributes</span></span>

<span data-ttu-id="607db-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="607db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="607db-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="607db-110">Child elements</span></span>

|<span data-ttu-id="607db-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="607db-111">**Element**</span></span>|<span data-ttu-id="607db-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="607db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="607db-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="607db-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="607db-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="607db-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="607db-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="607db-115">Parent elements</span></span>

<span data-ttu-id="607db-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="607db-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="607db-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="607db-117">Remarks</span></span>

<span data-ttu-id="607db-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="607db-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="607db-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="607db-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="607db-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="607db-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="607db-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="607db-121">Schema name</span></span>  <br/> |<span data-ttu-id="607db-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="607db-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="607db-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="607db-123">Validation file</span></span>  <br/> |<span data-ttu-id="607db-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="607db-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="607db-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="607db-125">Can be empty</span></span>  <br/> |<span data-ttu-id="607db-126">False</span><span class="sxs-lookup"><span data-stu-id="607db-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="607db-127">См. также</span><span class="sxs-lookup"><span data-stu-id="607db-127">See also</span></span>



- [<span data-ttu-id="607db-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="607db-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

