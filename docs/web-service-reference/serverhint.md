---
title: ServerHint
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerHint
api_type:
- schema
ms.assetid: 5ac60472-a565-43d1-a5fb-8be0c9511f82
description: Элемент ServerHint представляет собой отправную точку для отслеживания сообщений в удаленной сети или в лесу.
ms.openlocfilehash: 96953f70c239254d15b9d8173f951b52ca95a546
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835376"
---
# <a name="serverhint"></a><span data-ttu-id="5360f-103">ServerHint</span><span class="sxs-lookup"><span data-stu-id="5360f-103">ServerHint</span></span>

<span data-ttu-id="5360f-104">Элемент **ServerHint** представляет собой отправную точку для отслеживания сообщений в удаленной сети или в лесу.</span><span class="sxs-lookup"><span data-stu-id="5360f-104">The **ServerHint** element represents the starting point for tracking a message in a remote site or forest.</span></span> 
  
```xml
<ServerHint/>
```

 <span data-ttu-id="5360f-105">**string**</span><span class="sxs-lookup"><span data-stu-id="5360f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5360f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5360f-106">Attributes and elements</span></span>

<span data-ttu-id="5360f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5360f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5360f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5360f-108">Attributes</span></span>

<span data-ttu-id="5360f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5360f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5360f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5360f-110">Child elements</span></span>

<span data-ttu-id="5360f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5360f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5360f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5360f-112">Parent elements</span></span>

|<span data-ttu-id="5360f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5360f-113">**Element**</span></span>|<span data-ttu-id="5360f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5360f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5360f-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="5360f-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="5360f-116">Задает условия типам сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="5360f-116">Specifies criteria for the types of messages to find.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5360f-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5360f-117">Text value</span></span>

<span data-ttu-id="5360f-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="5360f-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5360f-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="5360f-119">Remarks</span></span>

<span data-ttu-id="5360f-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="5360f-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5360f-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5360f-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5360f-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5360f-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5360f-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5360f-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5360f-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5360f-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5360f-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5360f-125">Validation File</span></span>  <br/> |<span data-ttu-id="5360f-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5360f-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5360f-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5360f-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5360f-128">False</span><span class="sxs-lookup"><span data-stu-id="5360f-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5360f-129">См. также</span><span class="sxs-lookup"><span data-stu-id="5360f-129">See also</span></span>



[<span data-ttu-id="5360f-130">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="5360f-130">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)


- [<span data-ttu-id="5360f-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5360f-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

