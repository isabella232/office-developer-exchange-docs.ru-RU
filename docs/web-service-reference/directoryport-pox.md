---
title: Директорипорт (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ab436b54-ceba-4cd9-aeb4-134f9b93986d
description: Элемент Директорипорт указывает порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика услуг имен (NSPI).
ms.openlocfilehash: 1b73b9cd1d21c73f4e897684371993312f741322
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762109"
---
# <a name="directoryport-pox"></a><span data-ttu-id="4ee87-103">Директорипорт (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="4ee87-104">Элемент **директорипорт** указывает порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика услуг имен (NSPI).</span><span class="sxs-lookup"><span data-stu-id="4ee87-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="4ee87-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="4ee87-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="4ee87-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="4ee87-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="4ee87-109">Директорипорт (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4ee87-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4ee87-110">Attributes and elements</span></span>

<span data-ttu-id="4ee87-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4ee87-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ee87-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4ee87-112">Attributes</span></span>

<span data-ttu-id="4ee87-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ee87-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ee87-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4ee87-114">Child elements</span></span>

<span data-ttu-id="4ee87-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="4ee87-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4ee87-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4ee87-116">Parent elements</span></span>

|<span data-ttu-id="4ee87-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4ee87-117">**Element**</span></span>|<span data-ttu-id="4ee87-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4ee87-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ee87-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="4ee87-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4ee87-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4ee87-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4ee87-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4ee87-121">Text value</span></span>

<span data-ttu-id="4ee87-122">Текстовое значение представляет порт, используемый для доступа к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="4ee87-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4ee87-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="4ee87-123">Remarks</span></span>

<span data-ttu-id="4ee87-124">Элемент **директорипорт** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен "сумме" или "expr".</span><span class="sxs-lookup"><span data-stu-id="4ee87-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4ee87-125">См. также</span><span class="sxs-lookup"><span data-stu-id="4ee87-125">See also</span></span>

- [<span data-ttu-id="4ee87-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="4ee87-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

