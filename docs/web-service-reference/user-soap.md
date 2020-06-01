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
ms.openlocfilehash: f151ffa8050a10cdbb4562471d815f8692596cc3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456348"
---
# <a name="user-soap"></a><span data-ttu-id="e5910-103">Пользователь (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-103">User (SOAP)</span></span>

<span data-ttu-id="e5910-104">Элемент **User** представляет идентификатор одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="e5910-104">The **User** element represents the identity of a single user.</span></span> 
  
```XML
<User>
    <LegacyDN/>
    <Mailbox/>
    <RequestedSettings/>
</User>
```

 <span data-ttu-id="e5910-105">**User**</span><span class="sxs-lookup"><span data-stu-id="e5910-105">**User**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5910-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5910-106">Attributes and elements</span></span>

<span data-ttu-id="e5910-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e5910-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5910-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5910-108">Attributes</span></span>

<span data-ttu-id="e5910-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5910-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5910-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5910-110">Child elements</span></span>

|<span data-ttu-id="e5910-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5910-111">**Element**</span></span>|<span data-ttu-id="e5910-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5910-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5910-113">LegacyDN (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-113">LegacyDN (SOAP)</span></span>](legacydn-soap.md) <br/> |<span data-ttu-id="e5910-114">Представляет альтернативное различающееся имя устаревшего почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="e5910-114">Represents the alternate mailbox legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="e5910-115">Почтовый ящик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-115">Mailbox (SOAP)</span></span>](mailbox-soap.md) <br/> |<span data-ttu-id="e5910-116">Содержит адрес электронной почты пользователя, которого требуется обнаружить.</span><span class="sxs-lookup"><span data-stu-id="e5910-116">Contains the e-mail address of the user to be discovered.</span></span>  <br/> |
|[<span data-ttu-id="e5910-117">Рекуестедсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-117">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="e5910-118">Содержит имена запрошенных параметров конфигурации.</span><span class="sxs-lookup"><span data-stu-id="e5910-118">Contains the names of the requested configuration settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e5910-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5910-119">Parent elements</span></span>

|<span data-ttu-id="e5910-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5910-120">**Element**</span></span>|<span data-ttu-id="e5910-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5910-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5910-122">Пользователи (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-122">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="e5910-123">Представляет коллекцию элементов **User** .</span><span class="sxs-lookup"><span data-stu-id="e5910-123">Represents a collection of **User** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5910-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e5910-124">Text value</span></span>

<span data-ttu-id="e5910-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e5910-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5910-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5910-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5910-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5910-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e5910-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5910-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e5910-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="e5910-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e5910-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5910-130">Validation File</span></span>  <br/> |<span data-ttu-id="e5910-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e5910-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e5910-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5910-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5910-133">True</span><span class="sxs-lookup"><span data-stu-id="e5910-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5910-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e5910-134">See also</span></span>



[<span data-ttu-id="e5910-135">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="e5910-136">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-136">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="e5910-137">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e5910-137">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

