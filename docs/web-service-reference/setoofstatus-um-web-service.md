---
title: SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 9fc0ea9c-7a98-4fd7-a90c-cf5639c63a3a
description: Элемент SetOofStatus определяет запрос для задания состояния единой системы обмена сообщениями об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.
ms.openlocfilehash: df28c98013e1d5c00ea120ce1aa342e9fc2c6f31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835447"
---
# <a name="setoofstatus-um-web-service"></a><span data-ttu-id="0adba-103">SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="0adba-103">SetOofStatus (UM web service)</span></span>

<span data-ttu-id="0adba-104">Элемент **SetOofStatus** определяет запрос для задания состояния единой системы обмена сообщениями об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.</span><span class="sxs-lookup"><span data-stu-id="0adba-104">The **SetOofStatus** element defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span> 
  
[<span data-ttu-id="0adba-105">SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="0adba-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="0adba-106">**Тип**</span><span class="sxs-lookup"><span data-stu-id="0adba-106">**Type**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0adba-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0adba-107">Attributes and elements</span></span>

<span data-ttu-id="0adba-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0adba-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0adba-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0adba-109">Attributes</span></span>

<span data-ttu-id="0adba-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="0adba-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0adba-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0adba-111">Child elements</span></span>

|<span data-ttu-id="0adba-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0adba-112">**Element**</span></span>|<span data-ttu-id="0adba-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0adba-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0adba-114">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="0adba-114">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md) <br/> |<span data-ttu-id="0adba-115">Определяет значение для использования в запросе [SetOofStatus операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="0adba-115">Defines a value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0adba-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0adba-116">Parent elements</span></span>

<span data-ttu-id="0adba-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="0adba-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0adba-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0adba-118">Text value</span></span>

<span data-ttu-id="0adba-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="0adba-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0adba-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0adba-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0adba-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0adba-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0adba-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0adba-122">Schema Name</span></span>  <br/> |<span data-ttu-id="0adba-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="0adba-123">Messages</span></span>  <br/> |
|<span data-ttu-id="0adba-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0adba-124">Validation File</span></span>  <br/> |<span data-ttu-id="0adba-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0adba-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0adba-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0adba-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="0adba-127">False</span><span class="sxs-lookup"><span data-stu-id="0adba-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0adba-128">См. также</span><span class="sxs-lookup"><span data-stu-id="0adba-128">See also</span></span>



[<span data-ttu-id="0adba-129">Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="0adba-129">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
  
[<span data-ttu-id="0adba-130">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="0adba-130">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

