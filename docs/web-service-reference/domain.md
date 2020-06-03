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
ms.openlocfilehash: 3bf8e132b5fa588171ac4f3c095692bc68394663
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461333"
---
# <a name="domain"></a><span data-ttu-id="c296b-103">Домен</span><span class="sxs-lookup"><span data-stu-id="c296b-103">Domain</span></span>

<span data-ttu-id="c296b-104">Элемент **domain** определяет один домен SMTP.</span><span class="sxs-lookup"><span data-stu-id="c296b-104">The **Domain** element identifies a single SMTP domain.</span></span> 
  
```xml
<Domain Name="" IncludeSubdomains="" />
```

 <span data-ttu-id="c296b-105">**стмпдомаин**</span><span class="sxs-lookup"><span data-stu-id="c296b-105">**StmpDomain**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c296b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c296b-106">Attributes and elements</span></span>

<span data-ttu-id="c296b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c296b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c296b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c296b-108">Attributes</span></span>

|<span data-ttu-id="c296b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c296b-109">**Attribute**</span></span>|<span data-ttu-id="c296b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c296b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c296b-111">Имя</span><span class="sxs-lookup"><span data-stu-id="c296b-111">Name</span></span>  <br/> |<span data-ttu-id="c296b-112">Определяет имя домена.</span><span class="sxs-lookup"><span data-stu-id="c296b-112">Identifies the name of a domain.</span></span> <span data-ttu-id="c296b-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="c296b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="c296b-114">инклудесубдомаинс</span><span class="sxs-lookup"><span data-stu-id="c296b-114">IncludeSubdomains</span></span>  <br/> |<span data-ttu-id="c296b-115">Указывает, считаются ли внутренние домены домена, идентифицируемые атрибутом **Name** .</span><span class="sxs-lookup"><span data-stu-id="c296b-115">Indicates whether subdomains of the domain identified by the **Name** attribute are considered internal.</span></span> <span data-ttu-id="c296b-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c296b-116">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c296b-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c296b-117">Child elements</span></span>

<span data-ttu-id="c296b-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c296b-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c296b-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c296b-119">Parent elements</span></span>

|<span data-ttu-id="c296b-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c296b-120">**Element**</span></span>|<span data-ttu-id="c296b-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c296b-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c296b-122">Имена внутренних доменов (Смтпдомаинлист)</span><span class="sxs-lookup"><span data-stu-id="c296b-122">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="c296b-123">Определяет список внутренних доменов SMTP Организации.</span><span class="sxs-lookup"><span data-stu-id="c296b-123">Identifies the list of internal SMTP domains of the organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c296b-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c296b-124">Text value</span></span>

<span data-ttu-id="c296b-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="c296b-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c296b-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="c296b-126">Remarks</span></span>

<span data-ttu-id="c296b-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c296b-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c296b-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c296b-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c296b-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c296b-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c296b-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c296b-130">Schema Name</span></span>  <br/> |<span data-ttu-id="c296b-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c296b-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="c296b-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c296b-132">Validation File</span></span>  <br/> |<span data-ttu-id="c296b-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c296b-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c296b-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c296b-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="c296b-135">False</span><span class="sxs-lookup"><span data-stu-id="c296b-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c296b-136">См. также</span><span class="sxs-lookup"><span data-stu-id="c296b-136">See also</span></span>

- [<span data-ttu-id="c296b-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c296b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

