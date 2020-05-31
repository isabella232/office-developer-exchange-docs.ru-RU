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
ms.openlocfilehash: 6ecd23bc556ca32d724581a28cc7c117c6853207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762223"
---
# <a name="domainsettingerrors-soap"></a><span data-ttu-id="28203-103">Домаинсеттинжеррорс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28203-103">DomainSettingErrors (SOAP)</span></span>

<span data-ttu-id="28203-104">Элемент **домаинсеттингсеррорс** содержит сведения об ошибке для параметров, которые не могут быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="28203-104">The **DomainSettingsErrors** element contains error information for settings that could not be returned.</span></span> 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 <span data-ttu-id="28203-105">**домаинсеттингсеррорс**</span><span class="sxs-lookup"><span data-stu-id="28203-105">**DomainSettingsErrors**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28203-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28203-106">Attributes and elements</span></span>

<span data-ttu-id="28203-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="28203-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28203-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28203-108">Attributes</span></span>

<span data-ttu-id="28203-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28203-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28203-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28203-110">Child elements</span></span>

|<span data-ttu-id="28203-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28203-111">**Element**</span></span>|<span data-ttu-id="28203-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28203-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28203-113">Домаинсеттинжеррор (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28203-113">DomainSettingError (SOAP)</span></span>](domainsettingerror-soap.md) <br/> |<span data-ttu-id="28203-114">Представляет ошибку, возникшую при получении параметра домена.</span><span class="sxs-lookup"><span data-stu-id="28203-114">Represents an error that occurred while retrieving a domain setting.</span></span> <span data-ttu-id="28203-115">Представляет ошибку в запросе операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="28203-115">This represents an error from a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28203-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28203-116">Parent elements</span></span>

|<span data-ttu-id="28203-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="28203-117">**Element**</span></span>|<span data-ttu-id="28203-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="28203-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28203-119">Домаинреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28203-119">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="28203-120">Содержит запрошенные параметры для указанного домена.</span><span class="sxs-lookup"><span data-stu-id="28203-120">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="28203-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="28203-121">Text value</span></span>

<span data-ttu-id="28203-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="28203-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28203-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28203-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28203-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28203-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="28203-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28203-125">Schema Name</span></span>  <br/> |<span data-ttu-id="28203-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="28203-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="28203-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28203-127">Validation File</span></span>  <br/> |<span data-ttu-id="28203-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28203-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28203-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28203-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="28203-130">True</span><span class="sxs-lookup"><span data-stu-id="28203-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28203-131">См. также</span><span class="sxs-lookup"><span data-stu-id="28203-131">See also</span></span>

- [<span data-ttu-id="28203-132">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="28203-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

