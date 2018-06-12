---
title: Запрос (SOAP) (GetFederationInformation)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: Элемент запроса представляет запрос GetFederationInformationRequest (SOAP).
ms.openlocfilehash: 0fb9301c2f318aa2c27155675dd3c43b41aabecd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835119"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="315d3-103">Запрос (SOAP) (GetFederationInformation)</span><span class="sxs-lookup"><span data-stu-id="315d3-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="315d3-104">Элемент **запроса** представляет запрос [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="315d3-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="315d3-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="315d3-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="315d3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="315d3-106">Attributes and elements</span></span>

<span data-ttu-id="315d3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="315d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="315d3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="315d3-108">Attributes</span></span>

<span data-ttu-id="315d3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="315d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="315d3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="315d3-110">Child elements</span></span>

|<span data-ttu-id="315d3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="315d3-111">**Element**</span></span>|<span data-ttu-id="315d3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="315d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="315d3-113">Домен (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="315d3-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="315d3-114">Определяет домен, имеющей отношение доверия федерации.</span><span class="sxs-lookup"><span data-stu-id="315d3-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="315d3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="315d3-115">Parent elements</span></span>

|<span data-ttu-id="315d3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="315d3-116">**Element**</span></span>|<span data-ttu-id="315d3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="315d3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="315d3-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="315d3-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="315d3-119">Подготавливает звонка на сервере для запроса данных конфигурации для службы маркеров безопасности (STS).</span><span class="sxs-lookup"><span data-stu-id="315d3-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="315d3-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="315d3-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="315d3-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="315d3-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="315d3-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="315d3-122">Schema Name</span></span>  <br/> |<span data-ttu-id="315d3-123">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="315d3-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="315d3-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="315d3-124">Validation File</span></span>  <br/> |<span data-ttu-id="315d3-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="315d3-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="315d3-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="315d3-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="315d3-127">True</span><span class="sxs-lookup"><span data-stu-id="315d3-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="315d3-128">См. также</span><span class="sxs-lookup"><span data-stu-id="315d3-128">See also</span></span>



[<span data-ttu-id="315d3-129">Работа с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="315d3-129">Working with Autodiscover</span></span>](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

