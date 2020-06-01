---
title: Status (веб-служба единой системы обмена сообщениями — SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: Элемент Status определяет значение, которое будет использоваться в SetOofStatus операции (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459982"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="98c05-103">Status (веб-служба единой системы обмена сообщениями — SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="98c05-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="98c05-104">Элемент **Status** определяет значение, которое будет использоваться в [SetOofStatus операции (веб-служба единой системы обмена сообщениями)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="98c05-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="98c05-105">SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98c05-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="98c05-106">Status (веб-служба единой системы обмена сообщениями — SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="98c05-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="98c05-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="98c05-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="98c05-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98c05-108">Attributes and elements</span></span>

<span data-ttu-id="98c05-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="98c05-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98c05-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98c05-110">Attributes</span></span>

<span data-ttu-id="98c05-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98c05-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98c05-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98c05-112">Child elements</span></span>

<span data-ttu-id="98c05-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="98c05-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98c05-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98c05-114">Parent elements</span></span>

|<span data-ttu-id="98c05-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98c05-115">**Element**</span></span>|<span data-ttu-id="98c05-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98c05-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98c05-117">SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98c05-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="98c05-118">Определяет запрос на установку состояния единой системы обмена сообщениями (отсутствие на работе) для пользователя, который выполняет запрос.</span><span class="sxs-lookup"><span data-stu-id="98c05-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98c05-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="98c05-119">Text value</span></span>

<span data-ttu-id="98c05-120">Необходимо указать логическое значение.</span><span class="sxs-lookup"><span data-stu-id="98c05-120">A Boolean value is required.</span></span> <span data-ttu-id="98c05-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="98c05-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="98c05-122">Верно.</span><span class="sxs-lookup"><span data-stu-id="98c05-122">True</span></span>
    
- <span data-ttu-id="98c05-123">False</span><span class="sxs-lookup"><span data-stu-id="98c05-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="98c05-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="98c05-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="98c05-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="98c05-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="98c05-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="98c05-126">Schema Name</span></span>  <br/> |<span data-ttu-id="98c05-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="98c05-127">Messages</span></span>  <br/> |
|<span data-ttu-id="98c05-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="98c05-128">Validation File</span></span>  <br/> |<span data-ttu-id="98c05-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="98c05-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="98c05-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="98c05-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="98c05-131">False</span><span class="sxs-lookup"><span data-stu-id="98c05-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="98c05-132">См. также</span><span class="sxs-lookup"><span data-stu-id="98c05-132">See also</span></span>



[<span data-ttu-id="98c05-133">Операция SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="98c05-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

