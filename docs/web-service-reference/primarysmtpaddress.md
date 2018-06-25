---
title: Параметр PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: Элемент PrimarySmtpAddress представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, используемые для проверки подлинности сервер сервер или передача прав доступа.
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834881"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="12a48-103">Параметр PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="12a48-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="12a48-104">Элемент **PrimarySmtpAddress** представляет основной адрес Simple Mail Transfer Protocol (SMTP) учетной записи, используемые для проверки подлинности сервер сервер или передача прав доступа.</span><span class="sxs-lookup"><span data-stu-id="12a48-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="12a48-105">**PrimarySmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="12a48-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12a48-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="12a48-106">Attributes and elements</span></span>

<span data-ttu-id="12a48-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="12a48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12a48-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="12a48-108">Attributes</span></span>

<span data-ttu-id="12a48-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="12a48-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12a48-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="12a48-110">Child elements</span></span>

<span data-ttu-id="12a48-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="12a48-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12a48-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="12a48-112">Parent elements</span></span>

|<span data-ttu-id="12a48-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="12a48-113">**Element**</span></span>|<span data-ttu-id="12a48-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="12a48-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12a48-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="12a48-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="12a48-116">Представляет учетную запись для олицетворения при использовании заголовка ExchangeImpersonation SOAP.</span><span class="sxs-lookup"><span data-stu-id="12a48-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="12a48-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="12a48-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="12a48-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="12a48-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="12a48-119">Используется в заголовке SOAP для сериализации маркера проверки подлинности сервер сервер.</span><span class="sxs-lookup"><span data-stu-id="12a48-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="12a48-120">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="12a48-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="12a48-121">Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам.</span><span class="sxs-lookup"><span data-stu-id="12a48-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12a48-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="12a48-122">Text value</span></span>

<span data-ttu-id="12a48-123">Текстовое значение, представляющее SMTP-адрес является обязательным.</span><span class="sxs-lookup"><span data-stu-id="12a48-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12a48-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="12a48-124">Remarks</span></span>

<span data-ttu-id="12a48-125">Веб-служб Exchange необходимо определить, что почтовые ящики по основной SMTP-адрес почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="12a48-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="12a48-126">Прокси-сервер или альтернативные адреса, не принимаются.</span><span class="sxs-lookup"><span data-stu-id="12a48-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="12a48-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="12a48-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12a48-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="12a48-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12a48-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="12a48-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12a48-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="12a48-130">Schema Name</span></span>  <br/> |<span data-ttu-id="12a48-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="12a48-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="12a48-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="12a48-132">Validation File</span></span>  <br/> |<span data-ttu-id="12a48-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="12a48-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12a48-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="12a48-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="12a48-135">False</span><span class="sxs-lookup"><span data-stu-id="12a48-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12a48-136">См. также</span><span class="sxs-lookup"><span data-stu-id="12a48-136">See also</span></span>



- [<span data-ttu-id="12a48-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="12a48-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="12a48-138">Сервер сервер авторизации в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="12a48-138">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="12a48-139">Работа с делегированный доступ</span><span class="sxs-lookup"><span data-stu-id="12a48-139">Working with Delegate Access</span></span>](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

