---
title: Отклик (Жетдомаинсеттингс) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: Элемент Response представляет ответ на вызов Жетдомаинсеттингс для отдельного домена.
ms.openlocfilehash: 316d77104894cf5ed9121e7dab1c38646765c948
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835169"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="cabb1-103">Отклик (Жетдомаинсеттингс) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="cabb1-104">Элемент **Response** представляет ответ на вызов **жетдомаинсеттингс** для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="cabb1-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="cabb1-105">**жетдомаинсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="cabb1-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cabb1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cabb1-106">Attributes and elements</span></span>

<span data-ttu-id="cabb1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cabb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cabb1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cabb1-108">Attributes</span></span>

<span data-ttu-id="cabb1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="cabb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cabb1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cabb1-110">Child elements</span></span>

|<span data-ttu-id="cabb1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cabb1-111">**Element**</span></span>|<span data-ttu-id="cabb1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cabb1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cabb1-113">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="cabb1-114">Содержит ответ для каждого домена, запрошенного в запросе **жетдомаинсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="cabb1-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="cabb1-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="cabb1-116">Содержит код ошибки, связанный с ответом (если это требуется).</span><span class="sxs-lookup"><span data-stu-id="cabb1-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="cabb1-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="cabb1-118">Содержит сообщение об ошибке, связанное с ответом (если это требуется).</span><span class="sxs-lookup"><span data-stu-id="cabb1-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cabb1-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cabb1-119">Parent elements</span></span>

|<span data-ttu-id="cabb1-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cabb1-120">**Element**</span></span>|<span data-ttu-id="cabb1-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cabb1-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cabb1-122">Жетдомаинсеттингсреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="cabb1-123">Возврат к параметрам конфигурации домена, вызывающим абоненты.</span><span class="sxs-lookup"><span data-stu-id="cabb1-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cabb1-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cabb1-124">Text value</span></span>

<span data-ttu-id="cabb1-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="cabb1-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cabb1-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cabb1-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cabb1-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cabb1-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cabb1-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cabb1-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cabb1-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="cabb1-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cabb1-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cabb1-130">Validation File</span></span>  <br/> |<span data-ttu-id="cabb1-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cabb1-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cabb1-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cabb1-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cabb1-133">True</span><span class="sxs-lookup"><span data-stu-id="cabb1-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cabb1-134">См. также</span><span class="sxs-lookup"><span data-stu-id="cabb1-134">See also</span></span>



[<span data-ttu-id="cabb1-135">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cabb1-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

