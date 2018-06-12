---
title: Пользователь (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6bc0031-bc1d-41bd-84e4-9074a5b77012
description: Элемент User представляет идентификатор одного пользователя.
ms.openlocfilehash: a8dcb22f5c74a9622f978f34e48146115351fe82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840411"
---
# <a name="user-soap"></a><span data-ttu-id="88349-103">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-103">User (SOAP)</span></span>

<span data-ttu-id="88349-104">Элемент **User** представляет идентификатор одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="88349-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="88349-105">**user**</span><span class="sxs-lookup"><span data-stu-id="88349-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88349-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88349-106">Attributes and elements</span></span>

<span data-ttu-id="88349-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="88349-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88349-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88349-108">Attributes</span></span>

<span data-ttu-id="88349-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="88349-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="88349-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88349-110">Child elements</span></span>

|<span data-ttu-id="88349-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88349-111">**Element**</span></span>|<span data-ttu-id="88349-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88349-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88349-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="88349-114">Представляет устаревшее различающееся имя альтернативного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="88349-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="88349-115">Почтовый ящик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="88349-116">Содержит адрес электронной почты пользователя, чтобы обнаружить.</span><span class="sxs-lookup"><span data-stu-id="88349-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="88349-117">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="88349-118">Содержит имена параметров запрошенные конфигурации.</span><span class="sxs-lookup"><span data-stu-id="88349-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88349-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88349-119">Parent elements</span></span>

|<span data-ttu-id="88349-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88349-120">**Element**</span></span>|<span data-ttu-id="88349-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88349-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88349-122">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="88349-123">Представляет коллекцию элементов **пользователя** .</span><span class="sxs-lookup"><span data-stu-id="88349-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="88349-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="88349-124">Text value</span></span>

<span data-ttu-id="88349-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="88349-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88349-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88349-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88349-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88349-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="88349-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88349-128">Schema Name</span></span>  <br/> |<span data-ttu-id="88349-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="88349-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="88349-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88349-130">Validation File</span></span>  <br/> |<span data-ttu-id="88349-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88349-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88349-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88349-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="88349-133">True</span><span class="sxs-lookup"><span data-stu-id="88349-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88349-134">См. также</span><span class="sxs-lookup"><span data-stu-id="88349-134">See also</span></span>



[<span data-ttu-id="88349-135">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="88349-136">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="88349-137">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="88349-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

