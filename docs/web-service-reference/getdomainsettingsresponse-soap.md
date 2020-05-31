---
title: Жетдомаинсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: Элемент Жетдомаинсеттингсреспонсе представляет ответ на операцию Жетдомаинсеттингс (SOAP), которая возвращает параметры домена.
ms.openlocfilehash: c4984c2c6c532fcbd45c1a75733e578f6d9491fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762758"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="6660f-103">Жетдомаинсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6660f-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="6660f-104">Элемент **жетдомаинсеттингсреспонсе** представляет ответ на [операцию жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), которая возвращает параметры домена.</span><span class="sxs-lookup"><span data-stu-id="6660f-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="6660f-105">**жетдомаинсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="6660f-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6660f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6660f-106">Attributes and elements</span></span>

<span data-ttu-id="6660f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6660f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6660f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6660f-108">Attributes</span></span>

<span data-ttu-id="6660f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6660f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6660f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6660f-110">Child elements</span></span>

|<span data-ttu-id="6660f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6660f-111">**Element**</span></span>|<span data-ttu-id="6660f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6660f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6660f-113">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6660f-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="6660f-114">Содержит массив ответов для каждого параметра запрашиваемого домена.</span><span class="sxs-lookup"><span data-stu-id="6660f-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="6660f-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6660f-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="6660f-116">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="6660f-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="6660f-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6660f-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="6660f-118">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="6660f-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6660f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6660f-119">Parent elements</span></span>

<span data-ttu-id="6660f-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="6660f-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6660f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6660f-121">Text value</span></span>

<span data-ttu-id="6660f-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="6660f-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6660f-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6660f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6660f-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6660f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6660f-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6660f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6660f-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="6660f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6660f-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6660f-127">Validation File</span></span>  <br/> |<span data-ttu-id="6660f-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6660f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6660f-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6660f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6660f-130">True</span><span class="sxs-lookup"><span data-stu-id="6660f-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6660f-131">См. также</span><span class="sxs-lookup"><span data-stu-id="6660f-131">See also</span></span>



[<span data-ttu-id="6660f-132">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6660f-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

