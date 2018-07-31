---
title: Account (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Элемент учетной записи определяет параметры учетной записи пользователя или содержит сообщения об ошибках.
ms.openlocfilehash: 6cd87e678b3a524a69f6dca4d6999a3cff22fa57
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353345"
---
# <a name="account-pox"></a><span data-ttu-id="03c7b-103">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-103">Account (POX)</span></span>

<span data-ttu-id="03c7b-104">Элемент **учетной записи** определяет параметры учетной записи пользователя или содержит сообщения об ошибках.</span><span class="sxs-lookup"><span data-stu-id="03c7b-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="03c7b-105">AutoDiscover (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="03c7b-106">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="03c7b-107">Account (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-107">Account (POX)</span></span>](account-pox.md)
  
```XML
<Account>
   <AccountType/>
   <Action/>
   <MicrosoftOnline/>
   <RedirectURL/>
   <RedirectAddr/>
   <Image/>
   <ServiceHome/>
   <Protocol/>
   <PublicFolderInformation/>
</Account>
```

<br/>

```XML
<Account> 
    <Error/> 
</Account>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="03c7b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03c7b-108">Attributes and elements</span></span>

<span data-ttu-id="03c7b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="03c7b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03c7b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03c7b-110">Attributes</span></span>

<span data-ttu-id="03c7b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="03c7b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03c7b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03c7b-112">Child elements</span></span>

|<span data-ttu-id="03c7b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03c7b-113">**Element**</span></span>|<span data-ttu-id="03c7b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03c7b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03c7b-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="03c7b-116">Представляет тип учетной записи.</span><span class="sxs-lookup"><span data-stu-id="03c7b-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="03c7b-118">Предоставляет сведения, используемые для определения того, требуется ли другой запрос службы автообнаружения для возврата сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="03c7b-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="03c7b-120">Содержит значение, которое указывает почтовый ящик пользователя размещается ли в Exchange Online или Exchange Online в составе Office 365.</span><span class="sxs-lookup"><span data-stu-id="03c7b-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-121">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="03c7b-122">Содержит URL-адрес компьютера, на котором работает Exchange Server, который имеет роль сервера клиентского доступа установлен, который следует использовать для получения параметров службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="03c7b-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-123">RedirectAddr (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="03c7b-124">Указывает адрес электронной почты, который следует использовать для последующего запроса службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="03c7b-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="03c7b-126">Содержит путь, используемый на отображение фирменной настройки качества изображения.</span><span class="sxs-lookup"><span data-stu-id="03c7b-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-127">ServiceHome (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="03c7b-128">Содержит URL-адрес домашней страницы поставщика услуг Интернета (поставщика услуг Интернета).</span><span class="sxs-lookup"><span data-stu-id="03c7b-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="03c7b-129">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="03c7b-130">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="03c7b-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-131">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="03c7b-132">Содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя.</span><span class="sxs-lookup"><span data-stu-id="03c7b-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="03c7b-133">Error (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="03c7b-134">Содержит возврату ошибки службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="03c7b-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03c7b-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03c7b-135">Parent elements</span></span>

|<span data-ttu-id="03c7b-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03c7b-136">**Element**</span></span>|<span data-ttu-id="03c7b-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03c7b-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03c7b-138">Response (POX)</span><span class="sxs-lookup"><span data-stu-id="03c7b-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="03c7b-139">Содержит ответ от службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="03c7b-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03c7b-140">См. также</span><span class="sxs-lookup"><span data-stu-id="03c7b-140">See also</span></span>

- [<span data-ttu-id="03c7b-141">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="03c7b-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

