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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840411"
---
# <a name="user-soap"></a><span data-ttu-id="fc728-103">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-103">User (SOAP)</span></span>

<span data-ttu-id="fc728-104">Элемент **User** представляет идентификатор одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc728-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="fc728-105">**User**</span><span class="sxs-lookup"><span data-stu-id="fc728-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc728-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc728-106">Attributes and elements</span></span>

<span data-ttu-id="fc728-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fc728-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc728-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc728-108">Attributes</span></span>

<span data-ttu-id="fc728-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc728-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc728-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc728-110">Child elements</span></span>

|<span data-ttu-id="fc728-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc728-111">**Element**</span></span>|<span data-ttu-id="fc728-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc728-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc728-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="fc728-114">Представляет альтернативное различающееся имя устаревшего почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="fc728-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="fc728-115">Почтовый ящик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="fc728-116">Содержит адрес электронной почты пользователя, которого требуется обнаружить.</span><span class="sxs-lookup"><span data-stu-id="fc728-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="fc728-117">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="fc728-118">Содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="fc728-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc728-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc728-119">Parent elements</span></span>

|<span data-ttu-id="fc728-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc728-120">**Element**</span></span>|<span data-ttu-id="fc728-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc728-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc728-122">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="fc728-123">Представляет коллекцию элементов **User** .</span><span class="sxs-lookup"><span data-stu-id="fc728-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc728-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc728-124">Text value</span></span>

<span data-ttu-id="fc728-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc728-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc728-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc728-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc728-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc728-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fc728-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc728-128">Schema Name</span></span>  <br/> |<span data-ttu-id="fc728-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="fc728-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fc728-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc728-130">Validation File</span></span>  <br/> |<span data-ttu-id="fc728-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fc728-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc728-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc728-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc728-133">True</span><span class="sxs-lookup"><span data-stu-id="fc728-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc728-134">См. также</span><span class="sxs-lookup"><span data-stu-id="fc728-134">See also</span></span>



[<span data-ttu-id="fc728-135">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="fc728-136">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="fc728-137">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fc728-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

