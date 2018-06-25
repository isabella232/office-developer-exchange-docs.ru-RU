---
title: UserSMIMECertificate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 66e6b4ba-368d-4469-bd47-e59441b7d64d
description: Элемент UserSMIMECertificate содержит значение, которое кодирует сертификат SMIME контакта.
ms.openlocfilehash: 8b16f6768e3324c6d725a976210b8f7652155bf5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840450"
---
# <a name="usersmimecertificate"></a><span data-ttu-id="119ef-103">UserSMIMECertificate</span><span class="sxs-lookup"><span data-stu-id="119ef-103">UserSMIMECertificate</span></span>

<span data-ttu-id="119ef-104">Элемент **UserSMIMECertificate** содержит значение, которое кодирует сертификат SMIME контакта.</span><span class="sxs-lookup"><span data-stu-id="119ef-104">The **UserSMIMECertificate** element contains a value that encodes a contact's SMIME certificate.</span></span> 
  
```XML
<UserSMIMECertificate/>
```

 <span data-ttu-id="119ef-105">**ArrayOfBinaryType**</span><span class="sxs-lookup"><span data-stu-id="119ef-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="119ef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="119ef-106">Attributes and elements</span></span>

<span data-ttu-id="119ef-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="119ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="119ef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="119ef-108">Attributes</span></span>

<span data-ttu-id="119ef-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="119ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="119ef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="119ef-110">Child elements</span></span>

|<span data-ttu-id="119ef-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="119ef-111">**Element name**</span></span>|<span data-ttu-id="119ef-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="119ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="119ef-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="119ef-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="119ef-114">Содержит значения кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="119ef-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="119ef-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="119ef-115">Parent elements</span></span>

|<span data-ttu-id="119ef-116">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="119ef-116">**Element name**</span></span>|<span data-ttu-id="119ef-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="119ef-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="119ef-118">Контакт</span><span class="sxs-lookup"><span data-stu-id="119ef-118">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="119ef-119">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="119ef-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="119ef-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="119ef-120">Text value</span></span>

<span data-ttu-id="119ef-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="119ef-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="119ef-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="119ef-122">Remarks</span></span>

<span data-ttu-id="119ef-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="119ef-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="119ef-124">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="119ef-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="119ef-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="119ef-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="119ef-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="119ef-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="119ef-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="119ef-127">Schema name</span></span>  <br/> |<span data-ttu-id="119ef-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="119ef-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="119ef-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="119ef-129">Validation file</span></span>  <br/> |<span data-ttu-id="119ef-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="119ef-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="119ef-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="119ef-131">Can be empty</span></span>  <br/> |<span data-ttu-id="119ef-132">False</span><span class="sxs-lookup"><span data-stu-id="119ef-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="119ef-133">См. также</span><span class="sxs-lookup"><span data-stu-id="119ef-133">See also</span></span>



- [<span data-ttu-id="119ef-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="119ef-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="119ef-135">Создание контактов (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="119ef-135">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

