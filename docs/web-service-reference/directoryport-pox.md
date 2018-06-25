---
title: DirectoryPort (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: Элемент DirectoryPort определяет порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика имя службы (NSPI).
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762109"
---
# <a name="directoryport-pox"></a><span data-ttu-id="1b428-103">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="1b428-104">Элемент **DirectoryPort** определяет порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика имя службы (NSPI).</span><span class="sxs-lookup"><span data-stu-id="1b428-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="1b428-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="1b428-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="1b428-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="1b428-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="1b428-109">DirectoryPort (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1b428-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b428-110">Attributes and elements</span></span>

<span data-ttu-id="1b428-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1b428-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b428-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b428-112">Attributes</span></span>

<span data-ttu-id="1b428-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="1b428-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b428-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b428-114">Child elements</span></span>

<span data-ttu-id="1b428-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="1b428-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1b428-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b428-116">Parent elements</span></span>

|<span data-ttu-id="1b428-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b428-117">**Element**</span></span>|<span data-ttu-id="1b428-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b428-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b428-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="1b428-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1b428-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1b428-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1b428-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1b428-121">Text value</span></span>

<span data-ttu-id="1b428-122">Текстовое значение представляет порт, используемый для доступа к Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1b428-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1b428-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="1b428-123">Remarks</span></span>

<span data-ttu-id="1b428-124">Элемент **DirectoryPort** используется только в том случае, когда элемент [Типа (POX)](type-pox.md) равняется EXCH или Выражение.</span><span class="sxs-lookup"><span data-stu-id="1b428-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1b428-125">См. также</span><span class="sxs-lookup"><span data-stu-id="1b428-125">See also</span></span>

- [<span data-ttu-id="1b428-126">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="1b428-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

