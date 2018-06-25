---
title: Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)
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
description: Элемент Status определяет значение для использования в запросе SetOofStatus операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835583"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="82372-103">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="82372-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="82372-104">Элемент **Status** определяет значение для использования в запросе [SetOofStatus операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="82372-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="82372-105">SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="82372-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="82372-106">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="82372-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="82372-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="82372-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82372-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="82372-108">Attributes and elements</span></span>

<span data-ttu-id="82372-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="82372-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82372-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="82372-110">Attributes</span></span>

<span data-ttu-id="82372-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="82372-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82372-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="82372-112">Child elements</span></span>

<span data-ttu-id="82372-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="82372-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82372-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="82372-114">Parent elements</span></span>

|<span data-ttu-id="82372-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="82372-115">**Element**</span></span>|<span data-ttu-id="82372-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="82372-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82372-117">SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="82372-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="82372-118">Определяет запрос для задания состояния единой системы обмена сообщениями об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.</span><span class="sxs-lookup"><span data-stu-id="82372-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82372-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="82372-119">Text value</span></span>

<span data-ttu-id="82372-120">Логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="82372-120">A Boolean value is required.</span></span> <span data-ttu-id="82372-121">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="82372-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="82372-122">Истина</span><span class="sxs-lookup"><span data-stu-id="82372-122">True</span></span>
    
- <span data-ttu-id="82372-123">Ложь</span><span class="sxs-lookup"><span data-stu-id="82372-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="82372-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="82372-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82372-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="82372-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82372-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="82372-126">Schema Name</span></span>  <br/> |<span data-ttu-id="82372-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="82372-127">Messages</span></span>  <br/> |
|<span data-ttu-id="82372-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="82372-128">Validation File</span></span>  <br/> |<span data-ttu-id="82372-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="82372-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82372-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="82372-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="82372-131">False</span><span class="sxs-lookup"><span data-stu-id="82372-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82372-132">См. также</span><span class="sxs-lookup"><span data-stu-id="82372-132">See also</span></span>



[<span data-ttu-id="82372-133">Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="82372-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

