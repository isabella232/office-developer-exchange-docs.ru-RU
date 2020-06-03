---
title: Домаинсеттинжеррорс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: Элемент Домаинсеттингсеррорс содержит сведения об ошибке для параметров, которые не могут быть возвращены.
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530707"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="24214-103">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24214-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="24214-104">Элемент **домаинсеттингсеррорс** содержит сведения об ошибке для параметров, которые не могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="24214-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="24214-105">**домаинсеттингсеррорс**</span><span class="sxs-lookup"><span data-stu-id="24214-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="24214-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="24214-106">Attributes and elements</span></span>

<span data-ttu-id="24214-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="24214-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="24214-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="24214-108">Attributes</span></span>

<span data-ttu-id="24214-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24214-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="24214-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="24214-110">Child elements</span></span>

|<span data-ttu-id="24214-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24214-111">**Element**</span></span>|<span data-ttu-id="24214-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24214-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24214-113">Домаинсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24214-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="24214-114">Представляет ошибку, возникшую при получении параметра домена.</span><span class="sxs-lookup"><span data-stu-id="24214-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="24214-115">Представляет ошибку в запросе операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="24214-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="24214-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="24214-116">Parent elements</span></span>

|<span data-ttu-id="24214-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="24214-117">**Element**</span></span>|<span data-ttu-id="24214-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="24214-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="24214-119">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24214-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="24214-120">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="24214-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="24214-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="24214-121">Text value</span></span>

<span data-ttu-id="24214-122">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="24214-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="24214-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="24214-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="24214-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="24214-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="24214-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="24214-125">Schema Name</span></span>  <br/> |<span data-ttu-id="24214-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="24214-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="24214-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="24214-127">Validation File</span></span>  <br/> |<span data-ttu-id="24214-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="24214-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="24214-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="24214-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="24214-130">True</span><span class="sxs-lookup"><span data-stu-id="24214-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="24214-131">См. также</span><span class="sxs-lookup"><span data-stu-id="24214-131">See also</span></span>

- [<span data-ttu-id="24214-132">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="24214-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

