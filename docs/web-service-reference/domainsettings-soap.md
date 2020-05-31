---
title: Домаинсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: Элемент Домаинсеттингс представляет параметры домена, которые были отправлены в запросе автообнаружения или возвращены ответом автообнаружения.
ms.openlocfilehash: 961051399dc8babd8cba6eeaf43456071d0f40a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762224"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="8d6a4-103">Домаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d6a4-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="8d6a4-104">Элемент **домаинсеттингс** представляет параметры домена, которые были отправлены в запросе автообнаружения или возвращены ответом автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="8d6a4-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="8d6a4-105">**домаинсеттингс**</span><span class="sxs-lookup"><span data-stu-id="8d6a4-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d6a4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8d6a4-106">Attributes and elements</span></span>

<span data-ttu-id="8d6a4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8d6a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d6a4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8d6a4-108">Attributes</span></span>

<span data-ttu-id="8d6a4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8d6a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d6a4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8d6a4-110">Child elements</span></span>

|<span data-ttu-id="8d6a4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d6a4-111">**Element**</span></span>|<span data-ttu-id="8d6a4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d6a4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d6a4-113">Домаинсеттинг (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d6a4-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="8d6a4-114">Содержит параметры домена, которые возвращаются запросом [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="8d6a4-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d6a4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8d6a4-115">Parent elements</span></span>

|<span data-ttu-id="8d6a4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d6a4-116">**Element**</span></span>|<span data-ttu-id="8d6a4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d6a4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d6a4-118">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d6a4-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="8d6a4-119">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="8d6a4-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d6a4-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8d6a4-120">Text value</span></span>

<span data-ttu-id="8d6a4-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="8d6a4-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d6a4-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8d6a4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d6a4-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8d6a4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8d6a4-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8d6a4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8d6a4-125">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="8d6a4-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8d6a4-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8d6a4-126">Validation File</span></span>  <br/> |<span data-ttu-id="8d6a4-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="8d6a4-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d6a4-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8d6a4-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d6a4-129">True</span><span class="sxs-lookup"><span data-stu-id="8d6a4-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d6a4-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8d6a4-130">See also</span></span>

- [<span data-ttu-id="8d6a4-131">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d6a4-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

