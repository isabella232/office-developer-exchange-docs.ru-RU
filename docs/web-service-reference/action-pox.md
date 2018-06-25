---
title: Действие (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Элемент Action приведены сведения, которые используются для определения того, требуется ли другой запрос службы автообнаружения для возврата сведений о конфигурации пользователя.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762499"
---
# <a name="action-pox"></a><span data-ttu-id="c6d7b-103">Действие (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-103">Action (POX)</span></span>

<span data-ttu-id="c6d7b-104">Элемент **Action** приведены сведения, которые используются для определения того, требуется ли другой запрос службы автообнаружения для возврата сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="c6d7b-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="c6d7b-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="c6d7b-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="c6d7b-108">Действие (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="c6d7b-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c6d7b-109">Attributes and elements</span></span>

<span data-ttu-id="c6d7b-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6d7b-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c6d7b-111">Attributes</span></span>

<span data-ttu-id="c6d7b-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6d7b-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c6d7b-113">Child elements</span></span>

<span data-ttu-id="c6d7b-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6d7b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c6d7b-115">Parent elements</span></span>

|<span data-ttu-id="c6d7b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c6d7b-116">**Element**</span></span>|<span data-ttu-id="c6d7b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6d7b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6d7b-118">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="c6d7b-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="c6d7b-119">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6d7b-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c6d7b-120">Text value</span></span>

<span data-ttu-id="c6d7b-121">Текстовое значение представляет ли другой запрос автообнаружения, требуемой для получения сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="c6d7b-122">В следующей таблице приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="c6d7b-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="c6d7b-123">**Value**</span></span>|<span data-ttu-id="c6d7b-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c6d7b-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6d7b-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="c6d7b-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="c6d7b-126">Если указано это значение элемент [RedirectUrl (POX)](redirecturl-pox.md) будет укажите URL-адрес сервера клиентского доступа для использования в последующих запросов автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="c6d7b-127">Клиентское приложение должны прекратить перенаправление после 10 перенаправлений.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="c6d7b-128">redirectAddr</span><span class="sxs-lookup"><span data-stu-id="c6d7b-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="c6d7b-129">Если указано это значение, элемент [RedirectAddr (POX)](redirectaddr-pox.md) будет укажите адрес электронной почты, который следует использовать для последующего запроса службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="c6d7b-130">settings</span><span class="sxs-lookup"><span data-stu-id="c6d7b-130">settings</span></span>  <br/> |<span data-ttu-id="c6d7b-131">Если указано это значение ответа службы автообнаружения содержит параметры, которые используются для настройки учетной записи.</span><span class="sxs-lookup"><span data-stu-id="c6d7b-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="c6d7b-132">Большинство параметров можно найти в элементе [Протокола (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d7b-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6d7b-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c6d7b-133">See also</span></span>

- [<span data-ttu-id="c6d7b-134">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="c6d7b-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

