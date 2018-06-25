---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: Элемент SmtpAddress содержит SMTP-адрес, назначенный хранилище сообщений общих папок, настраиваемый для пользователя.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835507"
---
# <a name="smtpaddress-pox"></a><span data-ttu-id="6e647-103">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-103">SmtpAddress (POX)</span></span>

<span data-ttu-id="6e647-104">Элемент **SmtpAddress** содержит SMTP-адрес, назначенный хранилище сообщений общих папок, настраиваемый для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e647-104">The **SmtpAddress** element contains the SMTP address assigned to the public folder message store configured for the user.</span></span> 
  
- [<span data-ttu-id="6e647-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="6e647-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="6e647-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="6e647-108">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
- [<span data-ttu-id="6e647-109">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-109">SmtpAddress (POX)</span></span>](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6e647-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e647-110">Attributes and elements</span></span>

<span data-ttu-id="6e647-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6e647-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e647-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e647-112">Attributes</span></span>

<span data-ttu-id="6e647-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e647-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e647-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e647-114">Child elements</span></span>

<span data-ttu-id="6e647-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e647-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e647-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e647-116">Parent elements</span></span>

|<span data-ttu-id="6e647-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e647-117">**Element**</span></span>|<span data-ttu-id="6e647-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e647-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e647-119">PublicFolderInformation (POX)</span><span class="sxs-lookup"><span data-stu-id="6e647-119">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md) <br/> |<span data-ttu-id="6e647-120">Содержит сведения, которые клиенты могут использовать для отправки запроса службы автообнаружения для получения сведений о общей папки для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e647-120">Contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e647-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6e647-121">Text value</span></span>

<span data-ttu-id="6e647-122">Текстовое значение представляет SMTP-адрес, назначенный хранилище общих папок, настроенных для пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e647-122">The text value represents the SMTP address assigned to the public folder store configured for the user.</span></span> <span data-ttu-id="6e647-123">SMTP-адреса можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса службы автообнаружения для обнаружения параметров общей папки.</span><span class="sxs-lookup"><span data-stu-id="6e647-123">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6e647-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e647-124">Remarks</span></span>

<span data-ttu-id="6e647-125">Элемент **SmtpAddress** является обязательным дочерним элементом элемента **PublicFolderInformation** .</span><span class="sxs-lookup"><span data-stu-id="6e647-125">The **SmtpAddress** element is a required child element of the **PublicFolderInformation** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6e647-126">См. также</span><span class="sxs-lookup"><span data-stu-id="6e647-126">See also</span></span>

- [<span data-ttu-id="6e647-127">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="6e647-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

