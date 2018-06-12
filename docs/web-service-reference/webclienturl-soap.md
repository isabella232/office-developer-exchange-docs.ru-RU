---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: Элемент WebClientUrl представляет URL-адрес веб-клиент Exchange.
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840502"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="d21ee-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="d21ee-104">Элемент **WebClientUrl** представляет URL-адрес веб-клиент Exchange.</span><span class="sxs-lookup"><span data-stu-id="d21ee-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="d21ee-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="d21ee-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="d21ee-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="d21ee-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="d21ee-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d21ee-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d21ee-109">Attributes and elements</span></span>

<span data-ttu-id="d21ee-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d21ee-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d21ee-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d21ee-111">Attributes</span></span>

<span data-ttu-id="d21ee-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="d21ee-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d21ee-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d21ee-113">Child elements</span></span>

|<span data-ttu-id="d21ee-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d21ee-114">**Element**</span></span>|<span data-ttu-id="d21ee-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d21ee-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d21ee-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="d21ee-117">Представляет метод проверки подлинности для использования при доступе к указанному URL-АДРЕСУ.</span><span class="sxs-lookup"><span data-stu-id="d21ee-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="d21ee-118">URL-адрес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="d21ee-119">Представляет веб-адрес, URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="d21ee-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d21ee-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d21ee-120">Parent elements</span></span>

|<span data-ttu-id="d21ee-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d21ee-121">**Element**</span></span>|<span data-ttu-id="d21ee-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d21ee-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d21ee-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="d21ee-124">Представляет параметр пользователя, который содержит коллекцию элементов **WebClientUrl** .</span><span class="sxs-lookup"><span data-stu-id="d21ee-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d21ee-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d21ee-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d21ee-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d21ee-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d21ee-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d21ee-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d21ee-128">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="d21ee-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d21ee-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d21ee-129">Validation File</span></span>  <br/> |<span data-ttu-id="d21ee-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d21ee-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d21ee-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d21ee-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d21ee-132">True</span><span class="sxs-lookup"><span data-stu-id="d21ee-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d21ee-133">См. также</span><span class="sxs-lookup"><span data-stu-id="d21ee-133">See also</span></span>



[<span data-ttu-id="d21ee-134">URL-адрес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="d21ee-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d21ee-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

