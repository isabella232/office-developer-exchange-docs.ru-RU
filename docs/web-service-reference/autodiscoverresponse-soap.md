---
title: AutodiscoverResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 203a5ac3-ebd0-4514-acbe-bc1c74638127
description: Элемент AutodiscoverResponse (SOAP) представляет базовый элемент для всех ответов, возвращаемые службой автообнаружения.
ms.openlocfilehash: b92a71deb77e2b1dee42d970e2dc43a56044487a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761534"
---
# <a name="autodiscoverresponse-soap"></a><span data-ttu-id="25cbf-103">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-103">AutodiscoverResponse (SOAP)</span></span>

<span data-ttu-id="25cbf-104">Элемент **AutodiscoverResponse (SOAP)** представляет базовый элемент для всех ответов, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="25cbf-104">The **AutodiscoverResponse (SOAP)** element represents the base element for all responses that are returned by the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="25cbf-105">AutodiscoverResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-105">AutodiscoverResponse (SOAP)</span></span>](autodiscoverresponse-soap.md)
  
```XML
<AutodiscoverResponse>
    <UserResponses/>
    <UserSettingErrors/>
    <UserSettings/>
</AutodiscoverResponse>

```

 <span data-ttu-id="25cbf-106">**AutodiscoverResponse**</span><span class="sxs-lookup"><span data-stu-id="25cbf-106">**AutodiscoverResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25cbf-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25cbf-107">Attributes and elements</span></span>

<span data-ttu-id="25cbf-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="25cbf-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25cbf-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25cbf-109">Attributes</span></span>

<span data-ttu-id="25cbf-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="25cbf-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25cbf-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25cbf-111">Child elements</span></span>

|<span data-ttu-id="25cbf-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25cbf-112">**Element**</span></span>|<span data-ttu-id="25cbf-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25cbf-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25cbf-114">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-114">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="25cbf-115">Представляет коллекцию элементов [Ответ пользователя (SOAP)](userresponse-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="25cbf-115">Represents a collection of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="25cbf-116">UserSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-116">UserSettingErrors (SOAP)</span></span>](usersettingerrors-soap.md) <br/> |<span data-ttu-id="25cbf-117">Представляет коллекцию элементов [UserSettingError (SOAP)](usersettingerror-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="25cbf-117">Represents a collection of [UserSettingError (SOAP)](usersettingerror-soap.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="25cbf-118">Параметры пользователя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-118">UserSettings (SOAP)</span></span>](usersettings-soap.md) <br/> |<span data-ttu-id="25cbf-119">Представляет коллекцию элементов [UserSetting (SOAP)](usersetting-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="25cbf-119">Represents a collection of [UserSetting (SOAP)](usersetting-soap.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="25cbf-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25cbf-120">Parent elements</span></span>

<span data-ttu-id="25cbf-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="25cbf-121">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="25cbf-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25cbf-122">Text value</span></span>

<span data-ttu-id="25cbf-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="25cbf-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25cbf-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25cbf-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25cbf-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25cbf-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="25cbf-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25cbf-126">Schema Name</span></span>  <br/> |<span data-ttu-id="25cbf-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="25cbf-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="25cbf-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25cbf-128">Validation File</span></span>  <br/> |<span data-ttu-id="25cbf-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="25cbf-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="25cbf-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25cbf-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="25cbf-131">True</span><span class="sxs-lookup"><span data-stu-id="25cbf-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25cbf-132">См. также</span><span class="sxs-lookup"><span data-stu-id="25cbf-132">See also</span></span>

- [<span data-ttu-id="25cbf-133">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="25cbf-134">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-134">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
- [<span data-ttu-id="25cbf-135">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="25cbf-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

