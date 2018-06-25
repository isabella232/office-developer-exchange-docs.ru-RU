---
title: Ответ пользователя (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5007b1ba-bfcc-40d7-b1cb-e32fbaf54ffd
description: Элемент ответ пользователя представляет ответ на запрос GetUserSettings для отдельного пользователя.
ms.openlocfilehash: 6fcd82e06916df5acdd317cb44161c1b69e58574
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840436"
---
# <a name="userresponse-soap"></a><span data-ttu-id="08a86-103">Ответ пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-103">UserResponse (SOAP)</span></span>

<span data-ttu-id="08a86-104">Элемент **ответ пользователя** представляет ответ на запрос GetUserSettings для отдельного пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a86-104">The **UserResponse** element represents a response to a GetUserSettings request for an individual user.</span></span> 
  
```XML
<UserResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <RedirectTarget/>
   <UserSettingErrors/>
   <UserSettings/>
</UserResponse>
```

 <span data-ttu-id="08a86-105">**Ответ пользователя**</span><span class="sxs-lookup"><span data-stu-id="08a86-105">**UserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08a86-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08a86-106">Attributes and elements</span></span>

<span data-ttu-id="08a86-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="08a86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08a86-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08a86-108">Attributes</span></span>

<span data-ttu-id="08a86-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="08a86-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08a86-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08a86-110">Child elements</span></span>

|<span data-ttu-id="08a86-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08a86-111">**Element**</span></span>|<span data-ttu-id="08a86-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08a86-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08a86-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="08a86-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="08a86-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="08a86-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="08a86-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="08a86-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="08a86-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="08a86-118">Содержит целевой перенаправления URL-адрес или адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="08a86-118">Contains the target of the redirection URL or email address.</span></span>  <br/> |
|[<span data-ttu-id="08a86-119">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-119">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="08a86-120">Представляет коллекцию сведений о параметрах, которые не будут получены.</span><span class="sxs-lookup"><span data-stu-id="08a86-120">Represents a collection of information about settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="08a86-121">Параметры пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-121">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="08a86-122">Запрошенный параметры пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a86-122">The requested settings for the user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08a86-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08a86-123">Parent elements</span></span>

|<span data-ttu-id="08a86-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08a86-124">**Element**</span></span>|<span data-ttu-id="08a86-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08a86-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08a86-126">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-126">ArrayOfUserResponse (SOAP)</span></span>](arrayofuserresponse-soap.md) <br/> |<span data-ttu-id="08a86-127">Содержит массив ответов пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a86-127">Contains an array of user responses.</span></span>  <br/> |
|[<span data-ttu-id="08a86-128">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="08a86-128">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="08a86-129">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="08a86-129">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="08a86-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08a86-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08a86-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08a86-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="08a86-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08a86-132">Schema Name</span></span>  <br/> |<span data-ttu-id="08a86-133">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="08a86-133">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="08a86-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08a86-134">Validation File</span></span>  <br/> |<span data-ttu-id="08a86-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="08a86-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08a86-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08a86-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="08a86-137">True</span><span class="sxs-lookup"><span data-stu-id="08a86-137">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08a86-138">См. также</span><span class="sxs-lookup"><span data-stu-id="08a86-138">See also</span></span>



[<span data-ttu-id="08a86-139">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="08a86-139">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

