---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835507"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="11165-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="11165-104">Элемент **SmtpAddress** содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.</span><span class="sxs-lookup"><span data-stu-id="11165-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="11165-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="11165-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="11165-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="11165-108">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="11165-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="11165-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11165-110">Attributes and elements</span></span>

<span data-ttu-id="11165-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11165-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11165-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11165-112">Attributes</span></span>

<span data-ttu-id="11165-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="11165-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11165-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11165-114">Child elements</span></span>

<span data-ttu-id="11165-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="11165-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="11165-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11165-116">Parent elements</span></span>

|<span data-ttu-id="11165-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11165-117">**Element**</span></span>|<span data-ttu-id="11165-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11165-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11165-119">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="11165-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="11165-120">Содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.</span><span class="sxs-lookup"><span data-stu-id="11165-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="11165-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="11165-121">Text value</span></span>

<span data-ttu-id="11165-122">Текстовое значение представляет SMTP-адрес, назначенный хранилищу общедоступных папок, настроенному для пользователя.</span><span class="sxs-lookup"><span data-stu-id="11165-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="11165-123">Этот SMTP-адрес можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса на автообнаружение для обнаружения параметров общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="11165-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="11165-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="11165-124">Remarks</span></span>

<span data-ttu-id="11165-125">Элемент **SmtpAddress** является обязательным дочерним элементом элемента **публикфолдеринформатион** .</span><span class="sxs-lookup"><span data-stu-id="11165-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="11165-126">См. также</span><span class="sxs-lookup"><span data-stu-id="11165-126">See also</span></span>

- [<span data-ttu-id="11165-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="11165-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

