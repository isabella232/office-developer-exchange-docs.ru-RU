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
ms.openlocfilehash: 67fe7aea4533058fa0df972e49a2069749dc258b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455585"
---
# <a name="response-getdomainsettings-soap"></a><span data-ttu-id="89b3c-103">Отклик (Жетдомаинсеттингс) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-103">Response (GetDomainSettings) (SOAP)</span></span>

<span data-ttu-id="89b3c-104">Элемент **Response** представляет ответ на вызов **жетдомаинсеттингс** для отдельного домена.</span><span class="sxs-lookup"><span data-stu-id="89b3c-104">The **Response** element represents the response to a **GetDomainSettings** call for an individual domain.</span></span> 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 <span data-ttu-id="89b3c-105">**жетдомаинсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="89b3c-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89b3c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89b3c-106">Attributes and elements</span></span>

<span data-ttu-id="89b3c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="89b3c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89b3c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89b3c-108">Attributes</span></span>

<span data-ttu-id="89b3c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89b3c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89b3c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89b3c-110">Child elements</span></span>

|<span data-ttu-id="89b3c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89b3c-111">**Element**</span></span>|<span data-ttu-id="89b3c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89b3c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89b3c-113">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="89b3c-114">Содержит ответ для каждого домена, запрошенного в запросе **жетдомаинсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="89b3c-114">Contains the response for each domain requested in a **GetDomainSettings** request.</span></span>  <br/> |
|[<span data-ttu-id="89b3c-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="89b3c-116">Содержит код ошибки, связанный с ответом (если это требуется).</span><span class="sxs-lookup"><span data-stu-id="89b3c-116">Contains the error code that is associated with the response, if applicable.</span></span>  <br/> |
|[<span data-ttu-id="89b3c-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="89b3c-118">Содержит сообщение об ошибке, связанное с ответом (если это требуется).</span><span class="sxs-lookup"><span data-stu-id="89b3c-118">Contains the error message that is associated with the response, if applicable.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89b3c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89b3c-119">Parent elements</span></span>

|<span data-ttu-id="89b3c-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89b3c-120">**Element**</span></span>|<span data-ttu-id="89b3c-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89b3c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89b3c-122">Жетдомаинсеттингсреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-122">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md) <br/> |<span data-ttu-id="89b3c-123">Возврат к параметрам конфигурации домена, вызывающим абоненты.</span><span class="sxs-lookup"><span data-stu-id="89b3c-123">Returns to the caller the domain configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89b3c-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="89b3c-124">Text value</span></span>

<span data-ttu-id="89b3c-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89b3c-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89b3c-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89b3c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89b3c-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89b3c-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="89b3c-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89b3c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="89b3c-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="89b3c-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="89b3c-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89b3c-130">Validation File</span></span>  <br/> |<span data-ttu-id="89b3c-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="89b3c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89b3c-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89b3c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="89b3c-133">True</span><span class="sxs-lookup"><span data-stu-id="89b3c-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89b3c-134">См. также</span><span class="sxs-lookup"><span data-stu-id="89b3c-134">See also</span></span>



[<span data-ttu-id="89b3c-135">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="89b3c-135">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

