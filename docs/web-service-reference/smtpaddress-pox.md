---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.
ms.openlocfilehash: 48703a11fb056967c6c76073c2e928d5f6efa264
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468644"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="788d5-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="788d5-104">Элемент **SmtpAddress** содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788d5-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="788d5-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="788d5-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="788d5-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="788d5-108">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="788d5-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="788d5-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="788d5-110">Attributes and elements</span></span>

<span data-ttu-id="788d5-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="788d5-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="788d5-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="788d5-112">Attributes</span></span>

<span data-ttu-id="788d5-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="788d5-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="788d5-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="788d5-114">Child elements</span></span>

<span data-ttu-id="788d5-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="788d5-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="788d5-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="788d5-116">Parent elements</span></span>

|<span data-ttu-id="788d5-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="788d5-117">**Element**</span></span>|<span data-ttu-id="788d5-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="788d5-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="788d5-119">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="788d5-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="788d5-120">Содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788d5-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="788d5-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="788d5-121">Text value</span></span>

<span data-ttu-id="788d5-122">Текстовое значение представляет SMTP-адрес, назначенный хранилищу общедоступных папок, настроенному для пользователя.</span><span class="sxs-lookup"><span data-stu-id="788d5-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="788d5-123">Этот SMTP-адрес можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса на автообнаружение для обнаружения параметров общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="788d5-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="788d5-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="788d5-124">Remarks</span></span>

<span data-ttu-id="788d5-125">Элемент **SmtpAddress** является обязательным дочерним элементом элемента **публикфолдеринформатион** .</span><span class="sxs-lookup"><span data-stu-id="788d5-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="788d5-126">См. также</span><span class="sxs-lookup"><span data-stu-id="788d5-126">See also</span></span>

- [<span data-ttu-id="788d5-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="788d5-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

