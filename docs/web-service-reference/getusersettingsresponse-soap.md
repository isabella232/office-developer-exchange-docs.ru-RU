---
title: GetUserSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: Элемент GetUserSettingsResponse представляет ответа на запрос GetUserSettings операции (SOAP).
ms.openlocfilehash: 24dbfb1582f628fd0130aa82ea5f1beedd31b156
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833705"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="1db84-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1db84-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="1db84-104">Элемент **GetUserSettingsResponse** представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1db84-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="1db84-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="1db84-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1db84-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1db84-106">Attributes and elements</span></span>

<span data-ttu-id="1db84-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1db84-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1db84-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1db84-108">Attributes</span></span>

<span data-ttu-id="1db84-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1db84-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1db84-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1db84-110">Child elements</span></span>

|<span data-ttu-id="1db84-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1db84-111">**Element**</span></span>|<span data-ttu-id="1db84-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1db84-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1db84-113">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1db84-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="1db84-114">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1db84-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1db84-115">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1db84-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="1db84-116">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1db84-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1db84-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1db84-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="1db84-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1db84-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1db84-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1db84-119">Parent elements</span></span>

<span data-ttu-id="1db84-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="1db84-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1db84-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1db84-121">Text value</span></span>

<span data-ttu-id="1db84-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="1db84-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1db84-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1db84-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1db84-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1db84-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1db84-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1db84-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1db84-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1db84-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1db84-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1db84-127">Validation File</span></span>  <br/> |<span data-ttu-id="1db84-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1db84-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1db84-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1db84-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="1db84-130">True</span><span class="sxs-lookup"><span data-stu-id="1db84-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1db84-131">См. также</span><span class="sxs-lookup"><span data-stu-id="1db84-131">See also</span></span>



[<span data-ttu-id="1db84-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1db84-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

