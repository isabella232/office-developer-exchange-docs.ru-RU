---
title: Запрос (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: Элемент запрос содержит параметры запрошенные конфигурации и к конечным пользователям.
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835125"
---
# <a name="request-soap"></a><span data-ttu-id="67f03-103">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-103">Request (SOAP)</span></span>

<span data-ttu-id="67f03-104">Элемент **запрос** содержит параметры запрошенные конфигурации и к конечным пользователям.</span><span class="sxs-lookup"><span data-stu-id="67f03-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="67f03-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="67f03-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67f03-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="67f03-106">Attributes and elements</span></span>

<span data-ttu-id="67f03-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="67f03-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67f03-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="67f03-108">Attributes</span></span>

<span data-ttu-id="67f03-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="67f03-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67f03-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="67f03-110">Child elements</span></span>

|<span data-ttu-id="67f03-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="67f03-111">**Element**</span></span>|<span data-ttu-id="67f03-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="67f03-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67f03-113">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="67f03-114">Представляет коллекцию адреса электронной почты пользователей, для которых требуется извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="67f03-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="67f03-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="67f03-116">Содержит имена параметров запрошенные конфигурации.</span><span class="sxs-lookup"><span data-stu-id="67f03-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="67f03-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="67f03-118">Указывает версию определенного сервера, который хотите использовать поставщик.</span><span class="sxs-lookup"><span data-stu-id="67f03-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67f03-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="67f03-119">Parent elements</span></span>

|<span data-ttu-id="67f03-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="67f03-120">**Element**</span></span>|<span data-ttu-id="67f03-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="67f03-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67f03-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="67f03-123">Представляет запрос [GetUserSettings операции (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="67f03-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67f03-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="67f03-124">Text value</span></span>

<span data-ttu-id="67f03-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="67f03-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67f03-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="67f03-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67f03-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="67f03-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="67f03-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="67f03-128">Schema Name</span></span>  <br/> |<span data-ttu-id="67f03-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="67f03-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="67f03-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="67f03-130">Validation File</span></span>  <br/> |<span data-ttu-id="67f03-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="67f03-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67f03-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="67f03-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="67f03-133">True</span><span class="sxs-lookup"><span data-stu-id="67f03-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67f03-134">См. также</span><span class="sxs-lookup"><span data-stu-id="67f03-134">See also</span></span>



[<span data-ttu-id="67f03-135">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67f03-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

