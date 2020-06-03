---
title: Публикфолдеринформатион (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: Элемент Публикфолдеринформатион содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457720"
---
# <a name="publicfolderinformation-pox"></a><span data-ttu-id="a2211-103">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-103">PublicFolderInformation (POX)</span></span>

<span data-ttu-id="a2211-104">Элемент **публикфолдеринформатион** содержит сведения, которые клиенты могут использовать для отправки запроса на автообнаружение для обнаружения сведений о общедоступных папках для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2211-104">The **PublicFolderInformation** element contains information that clients can use to send an Autodiscover request to discover public folder information for the user.</span></span> 
  
[<span data-ttu-id="a2211-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a2211-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a2211-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a2211-108">Публикфолдеринформатион (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-108">PublicFolderInformation (POX)</span></span>](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a2211-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a2211-109">Attributes and elements</span></span>

<span data-ttu-id="a2211-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a2211-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2211-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a2211-111">Attributes</span></span>

<span data-ttu-id="a2211-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a2211-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2211-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a2211-113">Child elements</span></span>

|<span data-ttu-id="a2211-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2211-114">**Element**</span></span>|<span data-ttu-id="a2211-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2211-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2211-116">SmtpAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-116">SmtpAddress (POX)</span></span>](smtpaddress-pox.md) <br/> |<span data-ttu-id="a2211-117">Содержит SMTP-адрес, назначенный хранилищу сообщений общедоступных папок, настроенному для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2211-117">Contains the SMTP address assigned to the public folder message store configured for the user.</span></span> <span data-ttu-id="a2211-118">Этот SMTP-адрес можно использовать в элементе [EMailAddress (POX)](emailaddress-pox.md) запроса на автообнаружение для обнаружения параметров общедоступных папок.</span><span class="sxs-lookup"><span data-stu-id="a2211-118">This SMTP address can be used in the [EMailAddress (POX)](emailaddress-pox.md) element of an Autodiscover request to discover public folder settings.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a2211-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a2211-119">Parent elements</span></span>

|<span data-ttu-id="a2211-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a2211-120">**Element**</span></span>|<span data-ttu-id="a2211-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a2211-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2211-122">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a2211-122">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="a2211-123">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="a2211-123">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a2211-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="a2211-124">Remarks</span></span>

<span data-ttu-id="a2211-125">Элемент **публикфолдеринформатион** является необязательным дочерним элементом элемента **Account** .</span><span class="sxs-lookup"><span data-stu-id="a2211-125">The **PublicFolderInformation** element is an optional child element of the **Account** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a2211-126">См. также</span><span class="sxs-lookup"><span data-stu-id="a2211-126">See also</span></span>



[<span data-ttu-id="a2211-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a2211-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

