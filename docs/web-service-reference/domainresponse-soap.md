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
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762207"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="c8b14-103">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="c8b14-104">Элемент **домаинреспонсе** содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="c8b14-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="c8b14-105">**домаинреспонсе**</span><span class="sxs-lookup"><span data-stu-id="c8b14-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8b14-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c8b14-106">Attributes and elements</span></span>

<span data-ttu-id="c8b14-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c8b14-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8b14-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c8b14-108">Attributes</span></span>

<span data-ttu-id="c8b14-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c8b14-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8b14-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c8b14-110">Child elements</span></span>

|<span data-ttu-id="c8b14-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c8b14-111">**Element**</span></span>|<span data-ttu-id="c8b14-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c8b14-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8b14-113">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="c8b14-114">Содержит сведения об ошибках для параметров, которые не удалось вернуть.</span><span class="sxs-lookup"><span data-stu-id="c8b14-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="c8b14-115">Домаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="c8b14-116">Представляет параметры домена, которые были отправлены в запросе на обнаружение или возвращены ответом автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="c8b14-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="c8b14-117">Редиректтаржет (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="c8b14-118">Указывает целевой объект перенаправления.</span><span class="sxs-lookup"><span data-stu-id="c8b14-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="c8b14-119">Целевой может быть либо URL-адрес, либо адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c8b14-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="c8b14-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="c8b14-121">Указывает код ошибки, связанный с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="c8b14-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="c8b14-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="c8b14-123">Указывает сообщение об ошибке, связанное с конкретным запросом.</span><span class="sxs-lookup"><span data-stu-id="c8b14-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c8b14-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c8b14-124">Parent elements</span></span>

|<span data-ttu-id="c8b14-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c8b14-125">**Element**</span></span>|<span data-ttu-id="c8b14-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c8b14-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c8b14-127">Аррайофдомаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="c8b14-128">Содержит массив элементов **домаинреспонсе** .</span><span class="sxs-lookup"><span data-stu-id="c8b14-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="c8b14-129">Каждый элемент **домаинреспонсе** содержит запрошенные параметры для указанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c8b14-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="c8b14-130">Домаинреспонсес (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="c8b14-131">Содержит ответы для каждого домена.</span><span class="sxs-lookup"><span data-stu-id="c8b14-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c8b14-132">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c8b14-132">Text value</span></span>

<span data-ttu-id="c8b14-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="c8b14-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8b14-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c8b14-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8b14-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c8b14-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c8b14-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c8b14-136">Schema Name</span></span>  <br/> |<span data-ttu-id="c8b14-137">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="c8b14-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c8b14-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c8b14-138">Validation File</span></span>  <br/> |<span data-ttu-id="c8b14-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c8b14-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c8b14-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c8b14-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="c8b14-141">True</span><span class="sxs-lookup"><span data-stu-id="c8b14-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c8b14-142">См. также</span><span class="sxs-lookup"><span data-stu-id="c8b14-142">See also</span></span>

- [<span data-ttu-id="c8b14-143">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c8b14-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

