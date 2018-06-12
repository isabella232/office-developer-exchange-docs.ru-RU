---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: Элемент DomainSetting содержит параметры домена, возвращенных по запросу операции GetDomainSettings операции (SOAP).
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762219"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="01eab-103">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01eab-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="01eab-104">Элемент **DomainSetting** содержит параметры домена, возвращенных по запросу операции [операции GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="01eab-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="01eab-105">**DomainSetting**</span><span class="sxs-lookup"><span data-stu-id="01eab-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01eab-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="01eab-106">Attributes and elements</span></span>

<span data-ttu-id="01eab-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="01eab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01eab-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="01eab-108">Attributes</span></span>

<span data-ttu-id="01eab-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="01eab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01eab-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="01eab-110">Child elements</span></span>

|<span data-ttu-id="01eab-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01eab-111">**Element**</span></span>|<span data-ttu-id="01eab-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01eab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01eab-113">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01eab-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="01eab-114">Представляет имя параметра.</span><span class="sxs-lookup"><span data-stu-id="01eab-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01eab-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="01eab-115">Parent elements</span></span>

|<span data-ttu-id="01eab-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01eab-116">**Element**</span></span>|<span data-ttu-id="01eab-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01eab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01eab-118">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01eab-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="01eab-119">Представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="01eab-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01eab-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="01eab-120">Text value</span></span>

<span data-ttu-id="01eab-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="01eab-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01eab-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="01eab-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01eab-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="01eab-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="01eab-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="01eab-124">Schema Name</span></span>  <br/> |<span data-ttu-id="01eab-125">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="01eab-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="01eab-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="01eab-126">Validation File</span></span>  <br/> |<span data-ttu-id="01eab-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01eab-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01eab-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="01eab-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="01eab-129">True</span><span class="sxs-lookup"><span data-stu-id="01eab-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01eab-130">См. также</span><span class="sxs-lookup"><span data-stu-id="01eab-130">See also</span></span>

- [<span data-ttu-id="01eab-131">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01eab-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

