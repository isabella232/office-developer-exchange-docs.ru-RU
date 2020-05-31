---
title: Домаинсеттинг (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: Элемент Домаинсеттинг содержит параметры домена, которые возвращаются запросом операции Жетдомаинсеттингс (SOAP).
ms.openlocfilehash: f1c7a30ee221c5f3ca1358d0f3c3aca5c3467159
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762219"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="14ff1-103">Домаинсеттинг (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14ff1-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="14ff1-104">Элемент **домаинсеттинг** содержит параметры домена, которые возвращаются запросом операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="14ff1-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="14ff1-105">**домаинсеттинг**</span><span class="sxs-lookup"><span data-stu-id="14ff1-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="14ff1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="14ff1-106">Attributes and elements</span></span>

<span data-ttu-id="14ff1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="14ff1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="14ff1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="14ff1-108">Attributes</span></span>

<span data-ttu-id="14ff1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="14ff1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="14ff1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="14ff1-110">Child elements</span></span>

|<span data-ttu-id="14ff1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14ff1-111">**Element**</span></span>|<span data-ttu-id="14ff1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14ff1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14ff1-113">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14ff1-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="14ff1-114">Представляет имя параметра.</span><span class="sxs-lookup"><span data-stu-id="14ff1-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="14ff1-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="14ff1-115">Parent elements</span></span>

|<span data-ttu-id="14ff1-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="14ff1-116">**Element**</span></span>|<span data-ttu-id="14ff1-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="14ff1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="14ff1-118">Домаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14ff1-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="14ff1-119">Представляет параметры домена, которые были отправлены в запросе на обнаружение или возвращены ответом автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="14ff1-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="14ff1-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="14ff1-120">Text value</span></span>

<span data-ttu-id="14ff1-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="14ff1-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="14ff1-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="14ff1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="14ff1-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="14ff1-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="14ff1-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="14ff1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="14ff1-125">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="14ff1-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="14ff1-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="14ff1-126">Validation File</span></span>  <br/> |<span data-ttu-id="14ff1-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="14ff1-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="14ff1-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="14ff1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="14ff1-129">True</span><span class="sxs-lookup"><span data-stu-id="14ff1-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="14ff1-130">См. также</span><span class="sxs-lookup"><span data-stu-id="14ff1-130">See also</span></span>

- [<span data-ttu-id="14ff1-131">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="14ff1-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

