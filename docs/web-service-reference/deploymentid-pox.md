---
title: Деплойментид (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: b879c134-307e-4645-bb53-55d8ba4fad9c
description: Элемент Деплойментид однозначно идентифицирует лес Microsoft Exchange Server 2007.
ms.openlocfilehash: 4986a3404763e88fb3e84d52a5d30d54c810f93a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467923"
---
# <a name="deploymentid-pox"></a><span data-ttu-id="41168-103">Деплойментид (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-103">DeploymentId (POX)</span></span>

<span data-ttu-id="41168-104">Элемент **деплойментид** однозначно идентифицирует лес Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="41168-104">The **DeploymentId** element uniquely identifies the Microsoft Exchange Server 2007 forest.</span></span> 
  
- [<span data-ttu-id="41168-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="41168-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="41168-107">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-107">User (POX)</span></span>](user-pox.md)  
- [<span data-ttu-id="41168-108">Деплойментид (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-108">DeploymentId (POX)</span></span>](deploymentid-pox.md)
  
```xml
<DeploymentId/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="41168-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="41168-109">Attributes and elements</span></span>

<span data-ttu-id="41168-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="41168-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41168-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="41168-111">Attributes</span></span>

<span data-ttu-id="41168-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="41168-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41168-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="41168-113">Child elements</span></span>

<span data-ttu-id="41168-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="41168-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41168-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="41168-115">Parent elements</span></span>

|<span data-ttu-id="41168-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="41168-116">**Element**</span></span>|<span data-ttu-id="41168-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="41168-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41168-118">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="41168-118">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="41168-119">Предоставляет сведения, относящиеся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="41168-119">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41168-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="41168-120">Text value</span></span>

<span data-ttu-id="41168-121">Текстовое значение однозначно определяет лес Exchange 2007 в формате GUID.</span><span class="sxs-lookup"><span data-stu-id="41168-121">The text value uniquely identifies the Exchange 2007 forest in GUID format.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41168-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="41168-122">Remarks</span></span>

<span data-ttu-id="41168-123">Если вы удаляете и затем переустанавливаете Exchange 2007 и используете одно и то же имя сервера, значение **деплойментид** изменяется.</span><span class="sxs-lookup"><span data-stu-id="41168-123">If you uninstall and then reinstall Exchange 2007 and you use the same server name, the **DeploymentId** value changes.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="41168-124">См. также</span><span class="sxs-lookup"><span data-stu-id="41168-124">See also</span></span>

- [<span data-ttu-id="41168-125">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="41168-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

