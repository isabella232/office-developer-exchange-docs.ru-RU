---
title: SMTPLast (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f1aa8bd9-c6ac-41ac-8d2d-56fb20006005
description: Элемент SMTPLast указывает, требуется ли сервер Simple Mail Transfer Protocol (SMTP) загрузку электронной почты перед отправкой электронной почты с помощью SMTP-сервера.
ms.openlocfilehash: 5359f20b33855f4ef48566058bc46bd618e3b2ff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835505"
---
# <a name="smtplast-pox"></a><span data-ttu-id="33955-103">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-103">SMTPLast (POX)</span></span>

<span data-ttu-id="33955-104">Элемент **SMTPLast** указывает, требуется ли сервер Simple Mail Transfer Protocol (SMTP) загрузку электронной почты перед отправкой электронной почты с помощью SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="33955-104">The **SMTPLast** element specifies whether the Simple Mail Transfer Protocol (SMTP) server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> 
  
- [<span data-ttu-id="33955-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="33955-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="33955-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="33955-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="33955-109">SMTPLast (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-109">SMTPLast (POX)</span></span>](smtplast-pox.md)
  
```xml
<SMTPLast>on or off</SMTPLast>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="33955-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33955-110">Attributes and elements</span></span>

<span data-ttu-id="33955-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="33955-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33955-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33955-112">Attributes</span></span>

<span data-ttu-id="33955-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="33955-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33955-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33955-114">Child elements</span></span>

<span data-ttu-id="33955-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="33955-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33955-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33955-116">Parent elements</span></span>

|<span data-ttu-id="33955-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33955-117">**Element**</span></span>|<span data-ttu-id="33955-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33955-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33955-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="33955-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="33955-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="33955-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33955-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33955-121">Text value</span></span>

<span data-ttu-id="33955-122">Текстовое значение указывает, требуется ли SMTP-сервер загрузку электронной почты перед отправкой электронной почты с помощью SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="33955-122">The text value specifies whether the SMTP server requires that e-mail be downloaded before it sends e-mail by using the SMTP server.</span></span> <span data-ttu-id="33955-123">Возможные значения: **и **отключает**** .</span><span class="sxs-lookup"><span data-stu-id="33955-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="33955-124">**Значение по умолчанию отключен.**</span><span class="sxs-lookup"><span data-stu-id="33955-124">The default value is **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="33955-125">См. также</span><span class="sxs-lookup"><span data-stu-id="33955-125">See also</span></span>

- [<span data-ttu-id="33955-126">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="33955-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

