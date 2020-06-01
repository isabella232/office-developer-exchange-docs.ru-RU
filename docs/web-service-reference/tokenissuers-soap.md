---
title: Токениссуерс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Элементы Токениссуерс представляют коллекцию Токениссуер (SOAP).
ms.openlocfilehash: 352487ad3fd9c1ee7de756a109fb98a49d0cdcd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457076"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="ef6e5-103">Токениссуерс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ef6e5-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="ef6e5-104">Элементы **токениссуерс** представляют коллекцию [токениссуер (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ef6e5-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="ef6e5-105">**токениссуерс**</span><span class="sxs-lookup"><span data-stu-id="ef6e5-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ef6e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ef6e5-106">Attributes and elements</span></span>

<span data-ttu-id="ef6e5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ef6e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ef6e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ef6e5-108">Attributes</span></span>

<span data-ttu-id="ef6e5-109">Нет</span><span class="sxs-lookup"><span data-stu-id="ef6e5-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ef6e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ef6e5-110">Child elements</span></span>

|<span data-ttu-id="ef6e5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ef6e5-111">**Element**</span></span>|<span data-ttu-id="ef6e5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef6e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef6e5-113">Токениссуер (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ef6e5-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="ef6e5-114">Указывает [URI (SOAP)](uri-soap.md) и [конечную точку (SOAP)](endpoint-soap.md) для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="ef6e5-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ef6e5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ef6e5-115">Parent elements</span></span>

|<span data-ttu-id="ef6e5-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ef6e5-116">**Element**</span></span>|<span data-ttu-id="ef6e5-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ef6e5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ef6e5-118">Жетфедератионинформатионреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ef6e5-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="ef6e5-119">Содержит ответ [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ef6e5-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ef6e5-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="ef6e5-120">Remarks</span></span>

<span data-ttu-id="ef6e5-121">**Токениссуерс** представляет коллекцию элементов [токениссуер (SOAP)](tokenissuer-soap.md) , которые будут использоваться в автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="ef6e5-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="ef6e5-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ef6e5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ef6e5-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ef6e5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ef6e5-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ef6e5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ef6e5-125">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="ef6e5-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ef6e5-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ef6e5-126">Validation File</span></span>  <br/> |<span data-ttu-id="ef6e5-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ef6e5-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ef6e5-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ef6e5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ef6e5-129">True</span><span class="sxs-lookup"><span data-stu-id="ef6e5-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ef6e5-130">См. также</span><span class="sxs-lookup"><span data-stu-id="ef6e5-130">See also</span></span>



[<span data-ttu-id="ef6e5-131">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="ef6e5-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="ef6e5-132">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ef6e5-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

