---
title: Отключение (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: 2f8c1e8c-3bd4-4988-96b9-735c347b29f7
description: Элемент Disconnect определяет запрос на отключение вызова.
ms.openlocfilehash: 764532bdadd69caaa68406c84277197def3160af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762151"
---
# <a name="disconnect-um-web-service"></a><span data-ttu-id="a70a7-103">Отключение (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-103">Disconnect (UM web service)</span></span>

<span data-ttu-id="a70a7-104">Элемент **Disconnect** определяет запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="a70a7-104">The **Disconnect** element defines a request to disconnect a call.</span></span> 
  
- [<span data-ttu-id="a70a7-105">Отключение (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-105">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md)
  
```xml
<Disconnect>
  <CallId>   </CallId>
</Disconnect>
```

 <span data-ttu-id="a70a7-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="a70a7-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a70a7-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a70a7-107">Attributes and elements</span></span>

<span data-ttu-id="a70a7-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a70a7-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a70a7-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a70a7-109">Attributes</span></span>

<span data-ttu-id="a70a7-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="a70a7-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a70a7-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a70a7-111">Child elements</span></span>

|<span data-ttu-id="a70a7-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a70a7-112">**Element**</span></span>|<span data-ttu-id="a70a7-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a70a7-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a70a7-114">CallId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-114">CallId (UM web service)</span></span>](callid-um-web-service.md) <br/> |<span data-ttu-id="a70a7-115">Идентификатор вызова для отключения.</span><span class="sxs-lookup"><span data-stu-id="a70a7-115">The identifier of the call to disconnect.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a70a7-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a70a7-116">Parent elements</span></span>

<span data-ttu-id="a70a7-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="a70a7-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a70a7-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a70a7-118">Text value</span></span>

<span data-ttu-id="a70a7-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="a70a7-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a70a7-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a70a7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a70a7-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a70a7-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a70a7-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a70a7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="a70a7-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="a70a7-123">Messages</span></span>  <br/> |
|<span data-ttu-id="a70a7-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a70a7-124">Validation File</span></span>  <br/> |<span data-ttu-id="a70a7-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a70a7-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a70a7-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a70a7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="a70a7-127">False</span><span class="sxs-lookup"><span data-stu-id="a70a7-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a70a7-128">См. также</span><span class="sxs-lookup"><span data-stu-id="a70a7-128">See also</span></span>

- [<span data-ttu-id="a70a7-129">Операция отключения (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-129">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)  
- [<span data-ttu-id="a70a7-130">Операция PlayOnPhone (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-130">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md) 
- [<span data-ttu-id="a70a7-131">Операция PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-131">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)  
- [<span data-ttu-id="a70a7-132">CallId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="a70a7-132">CallId (UM web service)</span></span>](callid-um-web-service.md)

