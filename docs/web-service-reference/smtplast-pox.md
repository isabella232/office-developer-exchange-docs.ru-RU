---
title: Смтпласт (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: Элемент Смтпласт указывает, обязательно ли использовать SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера.
ms.openlocfilehash: 7019da28ffa196a9abc8798aa75aff2756198da3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468434"
---
# <a name="smtplast-pox"></a><span data-ttu-id="4931a-103">Смтпласт (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-103">SMTPLast (POX)</span></span>

<span data-ttu-id="4931a-104">Элемент **смтпласт** указывает, обязательно ли использовать SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="4931a-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="4931a-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="4931a-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="4931a-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="4931a-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="4931a-109">Смтпласт (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4931a-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4931a-110">Attributes and elements</span></span>

<span data-ttu-id="4931a-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4931a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4931a-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4931a-112">Attributes</span></span>

<span data-ttu-id="4931a-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4931a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4931a-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4931a-114">Child elements</span></span>

<span data-ttu-id="4931a-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4931a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4931a-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4931a-116">Parent elements</span></span>

|<span data-ttu-id="4931a-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4931a-117">**Element**</span></span>|<span data-ttu-id="4931a-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4931a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4931a-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="4931a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4931a-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4931a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4931a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4931a-121">Text value</span></span>

<span data-ttu-id="4931a-122">Текстовое значение указывает, требуется ли SMTP-сервер для загрузки электронной почты перед отправкой электронной почты с помощью SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="4931a-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="4931a-123">Возможные **значения:** **On и on** .</span><span class="sxs-lookup"><span data-stu-id="4931a-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="4931a-124">Значение по умолчанию — " **отключено**".</span><span class="sxs-lookup"><span data-stu-id="4931a-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4931a-125">См. также</span><span class="sxs-lookup"><span data-stu-id="4931a-125">See also</span></span>

- [<span data-ttu-id="4931a-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="4931a-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

