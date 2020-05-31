---
title: PrimarySmtpAddress
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
description: Элемент PrimarySmtpAddress представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер" или "делегированный доступ".
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834881"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="9196d-103">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="9196d-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="9196d-104">Элемент **PrimarySmtpAddress** представляет основной SMTP-адрес учетной записи, которая будет использоваться для авторизации "сервер-сервер" или "делегированный доступ".</span><span class="sxs-lookup"><span data-stu-id="9196d-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="9196d-105">**примарисмтпаддресстипе**</span><span class="sxs-lookup"><span data-stu-id="9196d-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9196d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9196d-106">Attributes and elements</span></span>

<span data-ttu-id="9196d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9196d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9196d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9196d-108">Attributes</span></span>

<span data-ttu-id="9196d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9196d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9196d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9196d-110">Child elements</span></span>

<span data-ttu-id="9196d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="9196d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9196d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9196d-112">Parent elements</span></span>

|<span data-ttu-id="9196d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9196d-113">**Element**</span></span>|<span data-ttu-id="9196d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9196d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9196d-115">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="9196d-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="9196d-116">Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="9196d-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="9196d-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9196d-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="9196d-118">сериализедсекуритиконтекст</span><span class="sxs-lookup"><span data-stu-id="9196d-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="9196d-119">Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".</span><span class="sxs-lookup"><span data-stu-id="9196d-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="9196d-120">UserId</span><span class="sxs-lookup"><span data-stu-id="9196d-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="9196d-121">Определяет делегата или пользователя с разрешениями на доступ к папке.</span><span class="sxs-lookup"><span data-stu-id="9196d-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9196d-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9196d-122">Text value</span></span>

<span data-ttu-id="9196d-123">Необходимо указать текстовое значение, представляющее SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="9196d-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9196d-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="9196d-124">Remarks</span></span>

<span data-ttu-id="9196d-125">Веб-службы Exchange требуют, чтобы почтовые ящики определялись основным SMTP-адресом почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="9196d-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="9196d-126">Прокси-сервер или альтернативные адреса не принимаются.</span><span class="sxs-lookup"><span data-stu-id="9196d-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="9196d-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9196d-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9196d-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9196d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9196d-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9196d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9196d-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9196d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="9196d-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9196d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="9196d-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9196d-132">Validation File</span></span>  <br/> |<span data-ttu-id="9196d-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9196d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9196d-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9196d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="9196d-135">False</span><span class="sxs-lookup"><span data-stu-id="9196d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9196d-136">См. также</span><span class="sxs-lookup"><span data-stu-id="9196d-136">See also</span></span>



- [<span data-ttu-id="9196d-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9196d-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9196d-138">Авторизация между серверами в EWS</span><span class="sxs-lookup"><span data-stu-id="9196d-138">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="9196d-139">Работа с делегированным доступом</span><span class="sxs-lookup"><span data-stu-id="9196d-139">Working with Delegate Access</span></span>](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

