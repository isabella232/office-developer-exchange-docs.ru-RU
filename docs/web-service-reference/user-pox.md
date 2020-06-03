---
title: Пользователь (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: Элемент User предоставляет сведения, относящиеся к пользователю.
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530220"
---
# <a name="user-pox"></a><span data-ttu-id="2d3d3-103">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-103">User (POX)</span></span>

<span data-ttu-id="2d3d3-104">Элемент **User** предоставляет сведения, относящиеся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="2d3d3-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2d3d3-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2d3d3-107">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2d3d3-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d3d3-108">Attributes and elements</span></span>

<span data-ttu-id="2d3d3-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d3d3-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d3d3-110">Attributes</span></span>

<span data-ttu-id="2d3d3-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d3d3-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d3d3-112">Child elements</span></span>

|<span data-ttu-id="2d3d3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d3d3-113">**Element**</span></span>|<span data-ttu-id="2d3d3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d3d3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d3d3-115">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="2d3d3-116">Представляет отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="2d3d3-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="2d3d3-118">Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="2d3d3-119">Деплойментид (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="2d3d3-120">Уникальный идентификатор леса Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="2d3d3-121">Аутодисковерсмтпаддресс (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="2d3d3-122">Содержит SMTP-адрес пользователя, который используется для процесса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d3d3-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d3d3-123">Parent elements</span></span>

|<span data-ttu-id="2d3d3-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d3d3-124">**Element**</span></span>|<span data-ttu-id="2d3d3-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d3d3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d3d3-126">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="2d3d3-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="2d3d3-127">Содержит ответ от службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d3d3-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="2d3d3-128">Remarks</span></span>

<span data-ttu-id="2d3d3-129">Запросы и ответы автообнаружения должны быть закодированы в кодировке UTF 8.</span><span class="sxs-lookup"><span data-stu-id="2d3d3-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="2d3d3-130">См. также</span><span class="sxs-lookup"><span data-stu-id="2d3d3-130">See also</span></span>



[<span data-ttu-id="2d3d3-131">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2d3d3-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

