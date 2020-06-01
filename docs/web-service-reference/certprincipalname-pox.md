---
title: ЦертпринЦипалнаме (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a24092c9-58be-4008-92c4-68ec5c6c0fa6
description: Элемент ЦертпринЦипалнаме указывает имя участника сертификата SSL, необходимое для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.
ms.openlocfilehash: fb2a1c8577bce41945b669be56f2a94a2c4dca26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463344"
---
# <a name="certprincipalname-pox"></a><span data-ttu-id="00b8b-103">ЦертпринЦипалнаме (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-103">CertPrincipalName (POX)</span></span>

<span data-ttu-id="00b8b-104">Элемент **цертпринЦипалнаме** указывает имя участника сертификата SSL, необходимое для подключения к организации Microsoft Exchange Server 2007 с помощью протокола SSL.</span><span class="sxs-lookup"><span data-stu-id="00b8b-104">The **CertPrincipalName** element specifies the Secure Sockets Layer (SSL) certificate principal name that is required to connect to the Microsoft Exchange Server 2007 organization by using SSL.</span></span> 
  
[<span data-ttu-id="00b8b-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="00b8b-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="00b8b-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="00b8b-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="00b8b-109">ЦертпринЦипалнаме (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-109">CertPrincipalName (POX)</span></span>](certprincipalname-pox.md)
  
```xml
<CertPrincipalName>none or servername</CertPrinicpalName>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="00b8b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="00b8b-110">Attributes and elements</span></span>

<span data-ttu-id="00b8b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="00b8b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00b8b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="00b8b-112">Attributes</span></span>

<span data-ttu-id="00b8b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="00b8b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00b8b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="00b8b-114">Child elements</span></span>

<span data-ttu-id="00b8b-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="00b8b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00b8b-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="00b8b-116">Parent elements</span></span>

|<span data-ttu-id="00b8b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="00b8b-117">**Element**</span></span>|<span data-ttu-id="00b8b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00b8b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00b8b-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="00b8b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="00b8b-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="00b8b-120">Contains the specifications for connecting a client to the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00b8b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="00b8b-121">Text value</span></span>

<span data-ttu-id="00b8b-122">Текстовое значение указывает имя субъекта сертификата SSL, которое требуется для подключения к организации Microsoft Exchange с помощью протокола SSL.</span><span class="sxs-lookup"><span data-stu-id="00b8b-122">The text value specifies the SSL certificate principal name that is required to connect to the Microsoft Exchange organization by using SSL.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00b8b-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="00b8b-123">Remarks</span></span>

<span data-ttu-id="00b8b-124">Если элемент **цертпринЦипалнаме** не указан, по умолчанию задается значение МССТД: Server, где Server — это значение, указанное в элементе [Server (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="00b8b-124">If the **CertPrincipalName** element is not specified, the default is set to msstd:SERVER, where SERVER is the value that is specified in the [Server (POX)](server-pox.md) element.</span></span> <span data-ttu-id="00b8b-125">Например, если параметр SERVER указан как example.com, а **цертпринЦипалнаме** остается пустым с включенным [протоколом SSL (POX)](ssl-pox.md) , значение по умолчанию **цертпринЦипалнаме** будет мсстд:ексампле. com.</span><span class="sxs-lookup"><span data-stu-id="00b8b-125">For example, if SERVER is specified as example.com and **CertPrincipalName** is left blank with [SSL (POX)](ssl-pox.md) turned on, the default value of **CertPrincipalName** would be msstd:example.com.</span></span> 
  
<span data-ttu-id="00b8b-126">Если **этот параметр не** указан, Windows будет проверять имя субъекта сертификата в соответствии с информацией, которая находится в разделе " [имена субъектов](https://go.microsoft.com/fwlink/?LinkId=93417) " на сайте MSDN.</span><span class="sxs-lookup"><span data-stu-id="00b8b-126">If **none** is specified, Windows will validate the certificate principal name according to information found in the [Principal Names](https://go.microsoft.com/fwlink/?LinkId=93417) topic on MSDN.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="00b8b-127">См. также</span><span class="sxs-lookup"><span data-stu-id="00b8b-127">See also</span></span>



[<span data-ttu-id="00b8b-128">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="00b8b-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

