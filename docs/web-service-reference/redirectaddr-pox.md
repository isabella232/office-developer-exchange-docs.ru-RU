---
title: Редиректаддр (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0e9fa6b6-7991-4dc1-a59a-48e5f8e041e4
description: Элемент Редиректаддр указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.
ms.openlocfilehash: fe15054b9962fc2decf52ac3c42536e36358948a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835020"
---
# <a name="redirectaddr-pox"></a><span data-ttu-id="d835c-103">Редиректаддр (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-103">RedirectAddr (POX)</span></span>

<span data-ttu-id="d835c-104">Элемент **редиректаддр** указывает адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="d835c-104">The **RedirectAddr** element specifies the e-mail address that should be used for a subsequent Autodiscover request.</span></span> 
  
[<span data-ttu-id="d835c-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d835c-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d835c-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d835c-108">Редиректаддр (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-108">RedirectAddr (POX)</span></span>](redirectaddr-pox.md)
  
```xml
<RedirectAddr/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d835c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d835c-109">Attributes and elements</span></span>

<span data-ttu-id="d835c-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d835c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d835c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d835c-111">Attributes</span></span>

<span data-ttu-id="d835c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="d835c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d835c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d835c-113">Child elements</span></span>

<span data-ttu-id="d835c-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="d835c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d835c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d835c-115">Parent elements</span></span>

|<span data-ttu-id="d835c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d835c-116">**Element**</span></span>|<span data-ttu-id="d835c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d835c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d835c-118">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="d835c-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="d835c-119">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="d835c-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d835c-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d835c-120">Text value</span></span>

<span data-ttu-id="d835c-121">Текстовое значение представляет адрес электронной почты, который будет использоваться для последующего запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="d835c-121">The text value represents the e-mail address that should be used for a subsequent Autodiscover request.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d835c-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="d835c-122">Remarks</span></span>

<span data-ttu-id="d835c-123">Если этот элемент присутствует в ответе автообнаружения, выполните другой запрос, используя текстовое значение элемента **редиректаддр** .</span><span class="sxs-lookup"><span data-stu-id="d835c-123">If this element is present in the Autodiscover response, make another request by using the text value of the **RedirectAddr** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d835c-124">См. также</span><span class="sxs-lookup"><span data-stu-id="d835c-124">See also</span></span>



[<span data-ttu-id="d835c-125">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="d835c-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

