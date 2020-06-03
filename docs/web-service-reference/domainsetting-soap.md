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
ms.openlocfilehash: 54441dd7cfcf7372807a1e6bfd8ea5d26805bffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526300"
---
# <a name="domainsetting-soap"></a><span data-ttu-id="961ad-103">Домаинсеттинг (SOAP)</span><span class="sxs-lookup"><span data-stu-id="961ad-103">DomainSetting (SOAP)</span></span>

<span data-ttu-id="961ad-104">Элемент **домаинсеттинг** содержит параметры домена, которые возвращаются запросом операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="961ad-104">The **DomainSetting** element contains domain settings that are returned by the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) operation request.</span></span> 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 <span data-ttu-id="961ad-105">**домаинсеттинг**</span><span class="sxs-lookup"><span data-stu-id="961ad-105">**DomainSetting**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="961ad-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="961ad-106">Attributes and elements</span></span>

<span data-ttu-id="961ad-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="961ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="961ad-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="961ad-108">Attributes</span></span>

<span data-ttu-id="961ad-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="961ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="961ad-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="961ad-110">Child elements</span></span>

|<span data-ttu-id="961ad-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="961ad-111">**Element**</span></span>|<span data-ttu-id="961ad-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="961ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="961ad-113">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="961ad-113">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="961ad-114">Представляет имя параметра.</span><span class="sxs-lookup"><span data-stu-id="961ad-114">Represents the name of a setting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="961ad-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="961ad-115">Parent elements</span></span>

|<span data-ttu-id="961ad-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="961ad-116">**Element**</span></span>|<span data-ttu-id="961ad-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="961ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="961ad-118">Домаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="961ad-118">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="961ad-119">Представляет параметры домена, которые были отправлены в запросе на обнаружение или возвращены ответом автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="961ad-119">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="961ad-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="961ad-120">Text value</span></span>

<span data-ttu-id="961ad-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="961ad-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="961ad-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="961ad-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="961ad-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="961ad-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="961ad-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="961ad-124">Schema Name</span></span>  <br/> |<span data-ttu-id="961ad-125">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="961ad-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="961ad-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="961ad-126">Validation File</span></span>  <br/> |<span data-ttu-id="961ad-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="961ad-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="961ad-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="961ad-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="961ad-129">True</span><span class="sxs-lookup"><span data-stu-id="961ad-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="961ad-130">См. также</span><span class="sxs-lookup"><span data-stu-id="961ad-130">See also</span></span>

- [<span data-ttu-id="961ad-131">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="961ad-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

