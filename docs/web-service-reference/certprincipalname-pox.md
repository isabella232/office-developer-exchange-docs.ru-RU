---
title: CertPrincipalName (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: Элемент CertPrincipalName указывает Secure Sockets Layer (SSL) имя участника сертификата, который необходим для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.
ms.openlocfilehash: d2766b16a3e8a1bcd013de332d9c07f709fcf949
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761676"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="53f8c-103">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="53f8c-104">Элемент **CertPrincipalName** указывает Secure Sockets Layer (SSL) имя участника сертификата, который необходим для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.</span><span class="sxs-lookup"><span data-stu-id="53f8c-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="53f8c-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="53f8c-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="53f8c-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="53f8c-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="53f8c-109">CertPrincipalName (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="53f8c-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="53f8c-110">Attributes and elements</span></span>

<span data-ttu-id="53f8c-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="53f8c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53f8c-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="53f8c-112">Attributes</span></span>

<span data-ttu-id="53f8c-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="53f8c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53f8c-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="53f8c-114">Child elements</span></span>

<span data-ttu-id="53f8c-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="53f8c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="53f8c-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="53f8c-116">Parent elements</span></span>

|<span data-ttu-id="53f8c-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="53f8c-117">**Element**</span></span>|<span data-ttu-id="53f8c-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="53f8c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53f8c-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="53f8c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="53f8c-120">Содержит спецификации для подключения клиентского компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="53f8c-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53f8c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="53f8c-121">Text value</span></span>

<span data-ttu-id="53f8c-122">Текстовое значение указывает имя участника сертификата SSL, которые требуются для подключения к Microsoft Exchange в организации с помощью протокола SSL.</span><span class="sxs-lookup"><span data-stu-id="53f8c-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53f8c-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="53f8c-123">Remarks</span></span>

<span data-ttu-id="53f8c-124">Если элемент **CertPrincipalName** не указан, по умолчанию имеет значение msstd:SERVER, где сервер — это значение, которое задано в элементе [Сервера (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="53f8c-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="53f8c-125">Например если сервер указан как example.com и **CertPrincipalName** оставлено пустым с включенным [SSL (POX)](ssl-pox.md) , значение по умолчанию **CertPrincipalName** будет msstd:example.com.</span><span class="sxs-lookup"><span data-stu-id="53f8c-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="53f8c-126">Если **он не задан,** Windows будет проверять имя участника сертификата в соответствии с сведения, содержащиеся в разделе [Имена участников](http://go.microsoft.com/fwlink/?LinkId=93417) на сайте MSDN.</span><span class="sxs-lookup"><span data-stu-id="53f8c-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](http://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="53f8c-127">См. также</span><span class="sxs-lookup"><span data-stu-id="53f8c-127">See also</span></span>



[<span data-ttu-id="53f8c-128">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="53f8c-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

