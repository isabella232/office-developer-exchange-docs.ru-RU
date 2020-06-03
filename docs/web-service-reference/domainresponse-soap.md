---
title: Домаинреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: Элемент Домаинреспонсе содержит запрошенные параметры для указанного домена.
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456964"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="bdf12-103">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="bdf12-104">Элемент **домаинреспонсе** содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="bdf12-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="bdf12-105">**домаинреспонсе**</span><span class="sxs-lookup"><span data-stu-id="bdf12-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bdf12-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bdf12-106">Attributes and elements</span></span>

<span data-ttu-id="bdf12-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bdf12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bdf12-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bdf12-108">Attributes</span></span>

<span data-ttu-id="bdf12-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bdf12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bdf12-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bdf12-110">Child elements</span></span>

|<span data-ttu-id="bdf12-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bdf12-111">**Element**</span></span>|<span data-ttu-id="bdf12-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bdf12-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdf12-113">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="bdf12-114">Содержит сведения об ошибках для параметров, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="bdf12-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="bdf12-115">Домаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="bdf12-116">Представляет параметры домена, которые были отправлены в запросе на обнаружение или возвращены ответом автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="bdf12-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="bdf12-117">Редиректтаржет (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="bdf12-118">Указывает целевой объект перенаправления.</span><span class="sxs-lookup"><span data-stu-id="bdf12-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="bdf12-119">Целевой может быть либо URL-адрес, либо адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bdf12-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="bdf12-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="bdf12-121">Указывает код ошибки, связанный с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="bdf12-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="bdf12-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="bdf12-123">Указывает сообщение об ошибке, связанное с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="bdf12-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bdf12-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bdf12-124">Parent elements</span></span>

|<span data-ttu-id="bdf12-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bdf12-125">**Element**</span></span>|<span data-ttu-id="bdf12-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bdf12-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bdf12-127">Аррайофдомаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="bdf12-128">Содержит массив элементов **домаинреспонсе** .</span><span class="sxs-lookup"><span data-stu-id="bdf12-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="bdf12-129">Каждый элемент **домаинреспонсе** содержит запрошенные параметры для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bdf12-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="bdf12-130">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="bdf12-131">Содержит ответы для каждого домена.</span><span class="sxs-lookup"><span data-stu-id="bdf12-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bdf12-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bdf12-132">Text value</span></span>

<span data-ttu-id="bdf12-133">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bdf12-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bdf12-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bdf12-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bdf12-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bdf12-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bdf12-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bdf12-136">Schema Name</span></span>  <br/> |<span data-ttu-id="bdf12-137">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bdf12-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bdf12-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bdf12-138">Validation File</span></span>  <br/> |<span data-ttu-id="bdf12-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bdf12-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bdf12-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bdf12-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="bdf12-141">True</span><span class="sxs-lookup"><span data-stu-id="bdf12-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bdf12-142">См. также</span><span class="sxs-lookup"><span data-stu-id="bdf12-142">See also</span></span>

- [<span data-ttu-id="bdf12-143">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bdf12-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

