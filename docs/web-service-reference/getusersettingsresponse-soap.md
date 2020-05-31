---
title: Жетусерсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: Элемент Жетусерсеттингсреспонсе представляет ответ на запрос операции GetUserSettings (SOAP).
ms.openlocfilehash: 24dbfb1582f628fd0130aa82ea5f1beedd31b156
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833705"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="3d34a-103">Жетусерсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3d34a-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="3d34a-104">Элемент **жетусерсеттингсреспонсе** представляет ответ на запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="3d34a-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="3d34a-105">**жетусерсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="3d34a-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3d34a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3d34a-106">Attributes and elements</span></span>

<span data-ttu-id="3d34a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3d34a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3d34a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3d34a-108">Attributes</span></span>

<span data-ttu-id="3d34a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d34a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3d34a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3d34a-110">Child elements</span></span>

|<span data-ttu-id="3d34a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d34a-111">**Element**</span></span>|<span data-ttu-id="3d34a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d34a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3d34a-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3d34a-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3d34a-114">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3d34a-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3d34a-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3d34a-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3d34a-116">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3d34a-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3d34a-117">Усерреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3d34a-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="3d34a-118">Содержит параметры конфигурации для каждого запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d34a-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3d34a-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3d34a-119">Parent elements</span></span>

<span data-ttu-id="3d34a-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d34a-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3d34a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3d34a-121">Text value</span></span>

<span data-ttu-id="3d34a-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="3d34a-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3d34a-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3d34a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3d34a-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3d34a-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3d34a-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3d34a-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3d34a-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="3d34a-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3d34a-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3d34a-127">Validation File</span></span>  <br/> |<span data-ttu-id="3d34a-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3d34a-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3d34a-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3d34a-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3d34a-130">True</span><span class="sxs-lookup"><span data-stu-id="3d34a-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3d34a-131">См. также</span><span class="sxs-lookup"><span data-stu-id="3d34a-131">See also</span></span>



[<span data-ttu-id="3d34a-132">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3d34a-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

