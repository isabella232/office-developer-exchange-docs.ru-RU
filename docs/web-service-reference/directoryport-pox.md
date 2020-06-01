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
ms.openlocfilehash: 2ba0a15cea0b4eb9b6069fab384edb3d9747a360
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462089"
---
# <a name="directoryport-pox"></a><span data-ttu-id="145ae-103">Директорипорт (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-103">DirectoryPort (POX)</span></span>

<span data-ttu-id="145ae-104">Элемент **директорипорт** указывает порт, используемый для подключения к каталогу при использовании протокола интерфейса поставщика услуг имен (NSPI).</span><span class="sxs-lookup"><span data-stu-id="145ae-104">The **DirectoryPort** element specifies the port that is used to connect to the directory when the Name Service Provider Interface (NSPI) protocol is used.</span></span> 
  
- [<span data-ttu-id="145ae-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="145ae-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="145ae-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="145ae-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="145ae-109">Директорипорт (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-109">DirectoryPort (POX)</span></span>](directoryport-pox.md)
  
```xml
<DirectoryPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="145ae-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="145ae-110">Attributes and elements</span></span>

<span data-ttu-id="145ae-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="145ae-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="145ae-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="145ae-112">Attributes</span></span>

<span data-ttu-id="145ae-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="145ae-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="145ae-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="145ae-114">Child elements</span></span>

<span data-ttu-id="145ae-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="145ae-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="145ae-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="145ae-116">Parent elements</span></span>

|<span data-ttu-id="145ae-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="145ae-117">**Element**</span></span>|<span data-ttu-id="145ae-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="145ae-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="145ae-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="145ae-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="145ae-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="145ae-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="145ae-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="145ae-121">Text value</span></span>

<span data-ttu-id="145ae-122">Текстовое значение представляет порт, используемый для доступа к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="145ae-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="145ae-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="145ae-123">Remarks</span></span>

<span data-ttu-id="145ae-124">Элемент **директорипорт** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен "сумме" или "expr".</span><span class="sxs-lookup"><span data-stu-id="145ae-124">The **DirectoryPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="145ae-125">См. также</span><span class="sxs-lookup"><span data-stu-id="145ae-125">See also</span></span>

- [<span data-ttu-id="145ae-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="145ae-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

