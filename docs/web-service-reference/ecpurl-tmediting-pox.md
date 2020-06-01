---
title: Екпурл-Тмедитинг (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 1fbc2ea9-3f94-441b-ab42-647326bf0021
description: Элемент Екпурл-Тмедитинг указывает на частичный URL-адрес, который можно сочетать со значением элемента Екпурл (POX) для создания URL-адреса, который можно использовать для изменения существующего почтового ящика сайта.
ms.openlocfilehash: 5d6c6b8e8f73d113cfde3570065435927ffbae05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463540"
---
# <a name="ecpurl-tmediting-pox"></a><span data-ttu-id="dedca-103">Екпурл-Тмедитинг (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-103">EcpUrl-tmEditing (POX)</span></span>

<span data-ttu-id="dedca-104">Элемент **екпурл-тмедитинг** указывает на частичный URL-адрес, который можно сочетать со значением элемента [екпурл (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для изменения существующего почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dedca-104">The **EcpUrl-tmEditing** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> 
  
[<span data-ttu-id="dedca-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="dedca-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="dedca-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="dedca-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="dedca-109">Екпурл-Тмедитинг (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-109">EcpUrl-tmEditing (POX)</span></span>](ecpurl-tmediting-pox.md)
  
```XML
<EcpUrl-tmEditing/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="dedca-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dedca-110">Attributes and elements</span></span>

<span data-ttu-id="dedca-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dedca-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dedca-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dedca-112">Attributes</span></span>

<span data-ttu-id="dedca-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dedca-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dedca-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dedca-114">Child elements</span></span>

<span data-ttu-id="dedca-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dedca-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dedca-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dedca-116">Parent elements</span></span>

|<span data-ttu-id="dedca-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dedca-117">**Element**</span></span>|<span data-ttu-id="dedca-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dedca-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dedca-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="dedca-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="dedca-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dedca-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dedca-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dedca-121">Text value</span></span>

<span data-ttu-id="dedca-122">Текстовое значение представляет собой частичный URL-адрес, который можно сочетать со значением элемента [екпурл (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для изменения существующего почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dedca-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to edit an existing site mailbox.</span></span> <span data-ttu-id="dedca-123">Значение элемента **екпурл — тмедитинг** содержит параметры, содержащиеся в символах "<" и ">", которые заменяются клиентом, как показано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="dedca-123">The value of the **EcpUrl-tmEditing** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="dedca-124">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="dedca-124">**Parameter**</span></span>|<span data-ttu-id="dedca-125">**Замена**</span><span class="sxs-lookup"><span data-stu-id="dedca-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="dedca-126">_Id_</span><span class="sxs-lookup"><span data-stu-id="dedca-126">_Id_</span></span> <br/> |<span data-ttu-id="dedca-127">SMTP-адрес электронной почты или различающееся имя для почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dedca-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dedca-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="dedca-128">Remarks</span></span>

<span data-ttu-id="dedca-129">Элемент **екпурл-тмедитинг** — необязательный дочерний элемент элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="dedca-129">The **EcpUrl-tmEditing** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dedca-130">См. также</span><span class="sxs-lookup"><span data-stu-id="dedca-130">See also</span></span>



[<span data-ttu-id="dedca-131">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="dedca-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

