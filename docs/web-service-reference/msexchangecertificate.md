---
title: MSExchangeCertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: Элемент MSExchangeCertificate содержит значение, которое кодирует сертификата Microsoft Exchange контакта.
ms.openlocfilehash: 8d07198012485b5c6d22e1fb4721890bf9a5eb39
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834498"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="f255b-103">MSExchangeCertificate</span><span class="sxs-lookup"><span data-stu-id="f255b-103">MSExchangeCertificate</span></span>

<span data-ttu-id="f255b-104">Элемент **MSExchangeCertificate** содержит значение, которое кодирует сертификата Microsoft Exchange контакта.</span><span class="sxs-lookup"><span data-stu-id="f255b-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="f255b-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="f255b-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f255b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f255b-106">Attributes and elements</span></span>

<span data-ttu-id="f255b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f255b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f255b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f255b-108">Attributes</span></span>

<span data-ttu-id="f255b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f255b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f255b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f255b-110">Child elements</span></span>

|<span data-ttu-id="f255b-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="f255b-111">**Element name**</span></span>|<span data-ttu-id="f255b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f255b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f255b-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="f255b-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="f255b-114">Содержит значения кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="f255b-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f255b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f255b-115">Parent elements</span></span>

|<span data-ttu-id="f255b-116">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="f255b-116">**Element name**</span></span>|<span data-ttu-id="f255b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f255b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f255b-118">Контакт</span><span class="sxs-lookup"><span data-stu-id="f255b-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f255b-119">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f255b-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f255b-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f255b-120">Text value</span></span>

<span data-ttu-id="f255b-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="f255b-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f255b-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="f255b-122">Remarks</span></span>

<span data-ttu-id="f255b-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f255b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="f255b-124">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="f255b-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f255b-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f255b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f255b-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f255b-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f255b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f255b-127">Schema name</span></span>  <br/> |<span data-ttu-id="f255b-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f255b-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="f255b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f255b-129">Validation file</span></span>  <br/> |<span data-ttu-id="f255b-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f255b-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f255b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f255b-131">Can be empty</span></span>  <br/> |<span data-ttu-id="f255b-132">False</span><span class="sxs-lookup"><span data-stu-id="f255b-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f255b-133">См. также</span><span class="sxs-lookup"><span data-stu-id="f255b-133">See also</span></span>



- [<span data-ttu-id="f255b-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f255b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f255b-135">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="f255b-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

