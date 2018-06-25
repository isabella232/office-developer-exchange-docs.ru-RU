---
title: PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 42b16880-1271-4690-abd0-0072d95b04b7
description: Элемент PlayOnPhoneResponse определяет ответа на запрос PlayOnPhone операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 482739d924bbac1d58624e50596af48cc405a3ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834832"
---
# <a name="playonphoneresponse-um-web-service"></a><span data-ttu-id="29365-103">PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="29365-103">PlayOnPhoneResponse (UM web service)</span></span>

<span data-ttu-id="29365-104">Элемент **PlayOnPhoneResponse** определяет ответ на запрос [операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="29365-104">The **PlayOnPhoneResponse** element defines a response to a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="29365-105">PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="29365-105">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
```xml
<PlayOnPhoneResponse />
```

 <span data-ttu-id="29365-106">**string**</span><span class="sxs-lookup"><span data-stu-id="29365-106">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29365-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="29365-107">Attributes and elements</span></span>

<span data-ttu-id="29365-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="29365-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29365-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="29365-109">Attributes</span></span>

<span data-ttu-id="29365-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="29365-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29365-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="29365-111">Child elements</span></span>

<span data-ttu-id="29365-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="29365-112">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="29365-113">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="29365-113">Parent elements</span></span>

<span data-ttu-id="29365-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="29365-114">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="29365-115">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="29365-115">Text value</span></span>

<span data-ttu-id="29365-116">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="29365-116">A text value is required.</span></span> <span data-ttu-id="29365-117">Текстовое значение является идентификатором звонка для значения [CallId (веб-служба единой системы обмена СООБЩЕНИЯМИ)](callid-um-web-service.md) в запрос [GetCallInfo операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](getcallinfo-operation-um-web-service.md) или в запросе на [операции отключения (веб-служба единой системы обмена СООБЩЕНИЯМИ)](disconnect-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="29365-117">The text value is the call identifier to use for the value of [CallId (UM web service)](callid-um-web-service.md) in a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request or a [Disconnect operation (UM web service)](disconnect-operation-um-web-service.md) request.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="29365-118">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="29365-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29365-119">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="29365-119">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29365-120">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="29365-120">Schema Name</span></span>  <br/> |<span data-ttu-id="29365-121">Сообщения</span><span class="sxs-lookup"><span data-stu-id="29365-121">Messages</span></span>  <br/> |
|<span data-ttu-id="29365-122">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="29365-122">Validation File</span></span>  <br/> |<span data-ttu-id="29365-123">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29365-123">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29365-124">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="29365-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="29365-125">False</span><span class="sxs-lookup"><span data-stu-id="29365-125">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29365-126">См. также</span><span class="sxs-lookup"><span data-stu-id="29365-126">See also</span></span>



[<span data-ttu-id="29365-127">Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="29365-127">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

