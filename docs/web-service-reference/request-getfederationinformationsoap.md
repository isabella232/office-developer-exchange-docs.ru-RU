---
title: Request (Жетфедератионинформатион) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: Элемент request представляет запрос Жетфедератионинформатионрекуест (SOAP).
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459583"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="5917b-103">Request (Жетфедератионинформатион) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5917b-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="5917b-104">Элемент **request** представляет запрос [жетфедератионинформатионрекуест (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="5917b-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="5917b-105">**жетфедератионинформатионрекуест**</span><span class="sxs-lookup"><span data-stu-id="5917b-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5917b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5917b-106">Attributes and elements</span></span>

<span data-ttu-id="5917b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5917b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5917b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5917b-108">Attributes</span></span>

<span data-ttu-id="5917b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5917b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5917b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5917b-110">Child elements</span></span>

|<span data-ttu-id="5917b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5917b-111">**Element**</span></span>|<span data-ttu-id="5917b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5917b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5917b-113">Домен (Жетфедератионинформатион) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5917b-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="5917b-114">Определяет домен, который имеет доверие федерации.</span><span class="sxs-lookup"><span data-stu-id="5917b-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5917b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5917b-115">Parent elements</span></span>

|<span data-ttu-id="5917b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5917b-116">**Element**</span></span>|<span data-ttu-id="5917b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5917b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5917b-118">Жетфедератионинформатионрекуестмессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="5917b-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="5917b-119">Подготавливает вызов к серверу для запроса данных конфигурации для службы маркеров безопасности (STS).</span><span class="sxs-lookup"><span data-stu-id="5917b-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="5917b-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5917b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5917b-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5917b-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="5917b-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5917b-122">Schema Name</span></span>  <br/> |<span data-ttu-id="5917b-123">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="5917b-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="5917b-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5917b-124">Validation File</span></span>  <br/> |<span data-ttu-id="5917b-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5917b-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5917b-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5917b-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="5917b-127">True</span><span class="sxs-lookup"><span data-stu-id="5917b-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5917b-128">См. также</span><span class="sxs-lookup"><span data-stu-id="5917b-128">See also</span></span>



[<span data-ttu-id="5917b-129">Работа со службой автообнаружения</span><span class="sxs-lookup"><span data-stu-id="5917b-129">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

