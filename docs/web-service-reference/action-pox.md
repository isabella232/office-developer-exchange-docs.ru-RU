---
title: Action (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a3462c6b-453c-462a-830d-f29ee4a2babb
description: Элемент Action предоставляет сведения, которые используются для определения того, требуется ли другой запрос автообнаружения для возврата сведений о конфигурации пользователя.
ms.openlocfilehash: 118bb59f2c929e3c74683dbf3f073da34d67a3e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762499"
---
# <a name="action-pox"></a><span data-ttu-id="2d1d1-103">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-103">Action (POX)</span></span>

<span data-ttu-id="2d1d1-104">Элемент **Action** предоставляет сведения, которые используются для определения того, требуется ли другой запрос автообнаружения для возврата сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-104">The **Action** element provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span> 
  
- [<span data-ttu-id="2d1d1-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="2d1d1-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="2d1d1-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="2d1d1-108">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-108">Action (POX)</span></span>](action-pox.md)
  
```xml
<Action>redirectUrl or redirectAddr or settings</Action>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2d1d1-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d1d1-109">Attributes and elements</span></span>

<span data-ttu-id="2d1d1-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d1d1-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d1d1-111">Attributes</span></span>

<span data-ttu-id="2d1d1-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d1d1-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d1d1-113">Child elements</span></span>

<span data-ttu-id="2d1d1-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d1d1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d1d1-115">Parent elements</span></span>

|<span data-ttu-id="2d1d1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d1d1-116">**Element**</span></span>|<span data-ttu-id="2d1d1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d1d1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d1d1-118">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="2d1d1-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="2d1d1-119">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d1d1-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2d1d1-120">Text value</span></span>

<span data-ttu-id="2d1d1-121">Текстовое значение указывает, требуется ли другой запрос автообнаружения для получения сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-121">The text value represents whether another Autodiscover request is necessary to retrieve the user's configuration information.</span></span> <span data-ttu-id="2d1d1-122">В приведенной ниже таблице перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-122">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="2d1d1-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="2d1d1-123">**Value**</span></span>|<span data-ttu-id="2d1d1-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d1d1-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2d1d1-125">redirectUrl</span><span class="sxs-lookup"><span data-stu-id="2d1d1-125">redirectUrl</span></span>  <br/> |<span data-ttu-id="2d1d1-126">Если задано это значение, элемент [redirectUrl адресом (POX)](redirecturl-pox.md) будет указывать URL-адрес сервера клиентского доступа, который будет использоваться в последующем запросе на обнаружение.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-126">If this value is specified, the [RedirectUrl (POX)](redirecturl-pox.md) element will specify the Client Access server URL to be used in the subsequent Autodiscover request.</span></span> <span data-ttu-id="2d1d1-127">Клиентское приложение должно прекратить перенаправление после 10 перенаправлений.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-127">The client application should stop redirecting after 10 redirects.</span></span>  <br/> |
|<span data-ttu-id="2d1d1-128">редиректаддр</span><span class="sxs-lookup"><span data-stu-id="2d1d1-128">redirectAddr</span></span>  <br/> |<span data-ttu-id="2d1d1-129">Если указано это значение, элемент [редиректаддр (POX)](redirectaddr-pox.md) будет указывать адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-129">If this value is specified, the [RedirectAddr (POX)](redirectaddr-pox.md) element will specify the e-mail address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|<span data-ttu-id="2d1d1-130">settings</span><span class="sxs-lookup"><span data-stu-id="2d1d1-130">settings</span></span>  <br/> |<span data-ttu-id="2d1d1-131">Если указано это значение, ответ автообнаружения содержит параметры, которые используются для настройки учетной записи.</span><span class="sxs-lookup"><span data-stu-id="2d1d1-131">If this value is specified, the Autodiscover response contains settings that are used to configure the account.</span></span> <span data-ttu-id="2d1d1-132">Большая часть параметров будет найдена в элементе [протокола (POX)](protocol-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="2d1d1-132">Most of the settings will be found in the [Protocol (POX)](protocol-pox.md) element.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d1d1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="2d1d1-133">See also</span></span>

- [<span data-ttu-id="2d1d1-134">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2d1d1-134">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

