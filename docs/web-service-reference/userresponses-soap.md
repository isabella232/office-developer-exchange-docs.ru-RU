---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: Элемент UserResponses содержит параметры конфигурации для каждого запрошенного пользователя.
ms.openlocfilehash: bee7f3c9a95c1facfe0adc990516dfa323d9c8cf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840435"
---
# <a name="userresponses-soap"></a><span data-ttu-id="bcad9-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bcad9-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="bcad9-104">Элемент **UserResponses** содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcad9-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="bcad9-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="bcad9-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bcad9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bcad9-106">Attributes and elements</span></span>

<span data-ttu-id="bcad9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bcad9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcad9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bcad9-108">Attributes</span></span>

<span data-ttu-id="bcad9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bcad9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcad9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bcad9-110">Child elements</span></span>

|<span data-ttu-id="bcad9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bcad9-111">**Element**</span></span>|<span data-ttu-id="bcad9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bcad9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcad9-113">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bcad9-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="bcad9-114">Представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcad9-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcad9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bcad9-115">Parent elements</span></span>

|<span data-ttu-id="bcad9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bcad9-116">**Element**</span></span>|<span data-ttu-id="bcad9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bcad9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcad9-118">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bcad9-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="bcad9-119">Содержит ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="bcad9-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="bcad9-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bcad9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcad9-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bcad9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bcad9-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bcad9-122">Schema Name</span></span>  <br/> |<span data-ttu-id="bcad9-123">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bcad9-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bcad9-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bcad9-124">Validation File</span></span>  <br/> |<span data-ttu-id="bcad9-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="bcad9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bcad9-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bcad9-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcad9-127">True</span><span class="sxs-lookup"><span data-stu-id="bcad9-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcad9-128">См. также</span><span class="sxs-lookup"><span data-stu-id="bcad9-128">See also</span></span>



[<span data-ttu-id="bcad9-129">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bcad9-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

