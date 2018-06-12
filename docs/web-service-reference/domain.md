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
description: Элемент домена определяет одного домена SMTP.
ms.openlocfilehash: 78eb1edfd347a513b84b9c15d143d76425041e85
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762206"
---
# <a name="domain"></a><span data-ttu-id="eae39-103">Домен</span><span class="sxs-lookup"><span data-stu-id="eae39-103">Domain</span></span>

<span data-ttu-id="eae39-104">Элемент **домена** определяет одного домена SMTP.</span><span class="sxs-lookup"><span data-stu-id="eae39-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="eae39-105">**StmpDomain**</span><span class="sxs-lookup"><span data-stu-id="eae39-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eae39-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eae39-106">Attributes and elements</span></span>

<span data-ttu-id="eae39-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eae39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eae39-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eae39-108">Attributes</span></span>

|<span data-ttu-id="eae39-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="eae39-109">**Attribute**</span></span>|<span data-ttu-id="eae39-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eae39-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eae39-111">Имя</span><span class="sxs-lookup"><span data-stu-id="eae39-111">Name</span></span>  <br/> |<span data-ttu-id="eae39-112">Определяет имя домена.</span><span class="sxs-lookup"><span data-stu-id="eae39-112">Identifies the name of a domain.</span></span> <span data-ttu-id="eae39-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="eae39-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="eae39-114">IncludeSubdomains</span><span class="sxs-lookup"><span data-stu-id="eae39-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="eae39-115">Указывает, считаются ли поддомены домена, определяемую средством атрибута **Name** внутренней.</span><span class="sxs-lookup"><span data-stu-id="eae39-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="eae39-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="eae39-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="eae39-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eae39-117">Child elements</span></span>

<span data-ttu-id="eae39-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="eae39-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eae39-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eae39-119">Parent elements</span></span>

|<span data-ttu-id="eae39-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eae39-120">**Element**</span></span>|<span data-ttu-id="eae39-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eae39-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eae39-122">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="eae39-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="eae39-123">Определяет список внутренних доменов SMTP организации.</span><span class="sxs-lookup"><span data-stu-id="eae39-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eae39-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="eae39-124">Text value</span></span>

<span data-ttu-id="eae39-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="eae39-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eae39-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="eae39-126">Remarks</span></span>

<span data-ttu-id="eae39-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="eae39-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eae39-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eae39-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eae39-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eae39-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eae39-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eae39-130">Schema Name</span></span>  <br/> |<span data-ttu-id="eae39-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="eae39-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="eae39-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eae39-132">Validation File</span></span>  <br/> |<span data-ttu-id="eae39-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eae39-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eae39-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eae39-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="eae39-135">False</span><span class="sxs-lookup"><span data-stu-id="eae39-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eae39-136">См. также</span><span class="sxs-lookup"><span data-stu-id="eae39-136">See also</span></span>

- [<span data-ttu-id="eae39-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="eae39-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

