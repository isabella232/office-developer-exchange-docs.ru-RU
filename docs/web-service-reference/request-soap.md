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
description: Элемент Request содержит запрошенные параметры конфигурации и целевые пользователи.
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44448991"
---
# <a name="request-soap"></a><span data-ttu-id="1b8d4-103">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-103">Request (SOAP)</span></span>

<span data-ttu-id="1b8d4-104">Элемент **request** содержит запрошенные параметры конфигурации и целевые пользователи.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="1b8d4-105">**жетусерсеттингсрекуест**</span><span class="sxs-lookup"><span data-stu-id="1b8d4-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b8d4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b8d4-106">Attributes and elements</span></span>

<span data-ttu-id="1b8d4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b8d4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b8d4-108">Attributes</span></span>

<span data-ttu-id="1b8d4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b8d4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b8d4-110">Child elements</span></span>

|<span data-ttu-id="1b8d4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b8d4-111">**Element**</span></span>|<span data-ttu-id="1b8d4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b8d4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b8d4-113">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="1b8d4-114">Представляет коллекцию адресов электронной почты пользователей, для которых необходимо извлечь параметры.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="1b8d4-115">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="1b8d4-116">Содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="1b8d4-117">Рекуестедверсион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="1b8d4-118">Указывает конкретную версию сервера, которую необходимо использовать поставщику.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b8d4-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b8d4-119">Parent elements</span></span>

|<span data-ttu-id="1b8d4-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b8d4-120">**Element**</span></span>|<span data-ttu-id="1b8d4-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b8d4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b8d4-122">Жетусерсеттингсрекуестмессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="1b8d4-123">Представляет запрос [операции GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1b8d4-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b8d4-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1b8d4-124">Text value</span></span>

<span data-ttu-id="1b8d4-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b8d4-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b8d4-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b8d4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b8d4-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b8d4-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1b8d4-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b8d4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1b8d4-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1b8d4-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1b8d4-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b8d4-130">Validation File</span></span>  <br/> |<span data-ttu-id="1b8d4-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1b8d4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b8d4-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b8d4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b8d4-133">True</span><span class="sxs-lookup"><span data-stu-id="1b8d4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b8d4-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1b8d4-134">See also</span></span>



[<span data-ttu-id="1b8d4-135">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b8d4-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

