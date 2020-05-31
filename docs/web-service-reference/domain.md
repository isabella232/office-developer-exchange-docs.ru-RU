---
title: Домен
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Domain
api_type:
- schema
ms.assetid: 7e45a061-856f-4b44-b053-a7c4d5ad569e
description: Элемент Domain определяет один домен SMTP.
ms.openlocfilehash: 78eb1edfd347a513b84b9c15d143d76425041e85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762206"
---
# <a name="domain"></a><span data-ttu-id="04557-103">Домен</span><span class="sxs-lookup"><span data-stu-id="04557-103">Domain</span></span>

<span data-ttu-id="04557-104">Элемент **domain** определяет один домен SMTP.</span><span class="sxs-lookup"><span data-stu-id="04557-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="04557-105">**стмпдомаин**</span><span class="sxs-lookup"><span data-stu-id="04557-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04557-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="04557-106">Attributes and elements</span></span>

<span data-ttu-id="04557-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="04557-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04557-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="04557-108">Attributes</span></span>

|<span data-ttu-id="04557-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="04557-109">**Attribute**</span></span>|<span data-ttu-id="04557-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04557-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="04557-111">Имя</span><span class="sxs-lookup"><span data-stu-id="04557-111">Name</span></span>  <br/> |<span data-ttu-id="04557-112">Определяет имя домена.</span><span class="sxs-lookup"><span data-stu-id="04557-112">Identifies the name of a domain.</span></span> <span data-ttu-id="04557-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="04557-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="04557-114">инклудесубдомаинс</span><span class="sxs-lookup"><span data-stu-id="04557-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="04557-115">Указывает, считаются ли внутренние домены домена, идентифицируемые атрибутом **Name** .</span><span class="sxs-lookup"><span data-stu-id="04557-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="04557-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="04557-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="04557-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="04557-117">Child elements</span></span>

<span data-ttu-id="04557-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="04557-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04557-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="04557-119">Parent elements</span></span>

|<span data-ttu-id="04557-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="04557-120">**Element**</span></span>|<span data-ttu-id="04557-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="04557-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04557-122">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="04557-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="04557-123">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="04557-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04557-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="04557-124">Text value</span></span>

<span data-ttu-id="04557-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="04557-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04557-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="04557-126">Remarks</span></span>

<span data-ttu-id="04557-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="04557-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04557-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="04557-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04557-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="04557-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04557-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="04557-130">Schema Name</span></span>  <br/> |<span data-ttu-id="04557-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="04557-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="04557-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="04557-132">Validation File</span></span>  <br/> |<span data-ttu-id="04557-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="04557-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04557-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="04557-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="04557-135">False</span><span class="sxs-lookup"><span data-stu-id="04557-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04557-136">См. также</span><span class="sxs-lookup"><span data-stu-id="04557-136">See also</span></span>

- [<span data-ttu-id="04557-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="04557-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

