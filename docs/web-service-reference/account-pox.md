---
title: Учетная запись (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 488fdbdc-e9d9-4301-91ab-e22eb42e549e
description: Элемент Account указывает параметры учетной записи пользователя или содержит ошибочные ответы.
ms.openlocfilehash: ffd8ebe4b7bd9d4b3f6a9b42fc557ac6189a068d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462320"
---
# <a name="account-pox"></a><span data-ttu-id="b473d-103">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-103">Account (POX)</span></span>

<span data-ttu-id="b473d-104">Элемент **Account** указывает параметры учетной записи пользователя или содержит ошибочные ответы.</span><span class="sxs-lookup"><span data-stu-id="b473d-104">The **Account** element specifies account settings for the user or contains error responses.</span></span> 
  
- [<span data-ttu-id="b473d-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
- [<span data-ttu-id="b473d-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="b473d-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-107">Account (POX)</span></span>](account-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="b473d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b473d-108">Attributes and elements</span></span>

<span data-ttu-id="b473d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b473d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b473d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b473d-110">Attributes</span></span>

<span data-ttu-id="b473d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b473d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b473d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b473d-112">Child elements</span></span>

|<span data-ttu-id="b473d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b473d-113">**Element**</span></span>|<span data-ttu-id="b473d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b473d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b473d-115">AccountType (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-115">AccountType (POX)</span></span>](accounttype-pox.md) <br/> |<span data-ttu-id="b473d-116">Представляет тип учетной записи.</span><span class="sxs-lookup"><span data-stu-id="b473d-116">Represents the account type.</span></span>  <br/> |
|[<span data-ttu-id="b473d-117">Action (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-117">Action (POX)</span></span>](action-pox.md) <br/> |<span data-ttu-id="b473d-118">Предоставляет сведения, используемые, чтобы определить, требуется ли другой запрос автообнаружения для возврата сведений о конфигурации пользователя.</span><span class="sxs-lookup"><span data-stu-id="b473d-118">Provides information that is used to determine whether another Autodiscover request is required to return the user configuration information.</span></span>  <br/> |
|[<span data-ttu-id="b473d-119">MicrosoftOnline (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-119">MicrosoftOnline (POX)</span></span>](microsoftonline-pox.md) <br/> |<span data-ttu-id="b473d-120">Содержит значение, указывающее, размещается ли почтовый ящик пользователя в Exchange Online или Exchange Online в составе Office 365.</span><span class="sxs-lookup"><span data-stu-id="b473d-120">Contains a value that indicates whether the user's mailbox is hosted in Exchange Online or Exchange Online as part of Office 365.</span></span>  <br/> |
|[<span data-ttu-id="b473d-121">RedirectUrl адресом (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-121">RedirectUrl (POX)</span></span>](redirecturl-pox.md) <br/> |<span data-ttu-id="b473d-122">Содержит URL-адрес компьютера, на котором установлен сервер Exchange с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b473d-122">Contains the URL of the computer that is running Exchange Server that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span>  <br/> |
|[<span data-ttu-id="b473d-123">Редиректаддр (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-123">RedirectAddr (POX)</span></span>](redirectaddr-pox.md) <br/> |<span data-ttu-id="b473d-124">Указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b473d-124">Specifies the email address that should be used for a subsequent Autodiscover request.</span></span>  <br/> |
|[<span data-ttu-id="b473d-125">Image (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-125">Image (POX)</span></span>](image-pox.md) <br/> |<span data-ttu-id="b473d-126">Содержит путь к изображению, используемому для фирменной настройки.</span><span class="sxs-lookup"><span data-stu-id="b473d-126">Contains the path of an image that is used to brand the configuration experience.</span></span>  <br/> |
|[<span data-ttu-id="b473d-127">Сервицехоме (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-127">ServiceHome (POX)</span></span>](servicehome-pox.md) <br/> |<span data-ttu-id="b473d-128">Содержит URL-адрес домашней страницы поставщика услуг Интернета.</span><span class="sxs-lookup"><span data-stu-id="b473d-128">Contains the URL of the home page of the Internet service provider (ISP).</span></span>  <br/> |
|[<span data-ttu-id="b473d-129">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-129">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b473d-130">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b473d-130">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
|[<span data-ttu-id="b473d-131">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-131">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="b473d-132">Содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.</span><span class="sxs-lookup"><span data-stu-id="b473d-132">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
|[<span data-ttu-id="b473d-133">Ошибка (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-133">Error (POX)</span></span>](error-pox.md) <br/> |<span data-ttu-id="b473d-134">Содержит ответ об ошибке автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b473d-134">Contains an Autodiscover error response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b473d-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b473d-135">Parent elements</span></span>

|<span data-ttu-id="b473d-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b473d-136">**Element**</span></span>|<span data-ttu-id="b473d-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b473d-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b473d-138">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="b473d-138">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="b473d-139">Содержит ответ от службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="b473d-139">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b473d-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b473d-140">See also</span></span>

- [<span data-ttu-id="b473d-141">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="b473d-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

