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
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840408"
---
# <a name="user-pox"></a><span data-ttu-id="0af0a-103">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-103">User (POX)</span></span>

<span data-ttu-id="0af0a-104">Элемент **User** предоставляет сведения, относящиеся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="0af0a-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="0af0a-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0af0a-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0af0a-107">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0af0a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0af0a-108">Attributes and elements</span></span>

<span data-ttu-id="0af0a-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0af0a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0af0a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0af0a-110">Attributes</span></span>

<span data-ttu-id="0af0a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0af0a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0af0a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0af0a-112">Child elements</span></span>

|<span data-ttu-id="0af0a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0af0a-113">**Element**</span></span>|<span data-ttu-id="0af0a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0af0a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0af0a-115">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="0af0a-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="0af0a-116">Представляет отображаемое имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="0af0a-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="0af0a-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="0af0a-118">Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.</span><span class="sxs-lookup"><span data-stu-id="0af0a-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="0af0a-119">Деплойментид (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="0af0a-120">Уникальный идентификатор леса Exchange.</span><span class="sxs-lookup"><span data-stu-id="0af0a-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="0af0a-121">Аутодисковерсмтпаддресс (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="0af0a-122">Содержит SMTP-адрес пользователя, который используется для процесса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0af0a-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0af0a-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0af0a-123">Parent elements</span></span>

|<span data-ttu-id="0af0a-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0af0a-124">**Element**</span></span>|<span data-ttu-id="0af0a-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0af0a-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0af0a-126">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="0af0a-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="0af0a-127">Содержит ответ от службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0af0a-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0af0a-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="0af0a-128">Remarks</span></span>

<span data-ttu-id="0af0a-129">Запросы и ответы автообнаружения должны быть закодированы в кодировке UTF 8.</span><span class="sxs-lookup"><span data-stu-id="0af0a-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0af0a-130">См. также</span><span class="sxs-lookup"><span data-stu-id="0af0a-130">See also</span></span>



[<span data-ttu-id="0af0a-131">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="0af0a-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

