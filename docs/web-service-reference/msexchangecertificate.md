---
title: мсексчанжецертификате
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c514f22f-be3e-4cad-ac56-bdff6bafcee6
description: Элемент Мсексчанжецертификате содержит значение, которое кодирует сертификат Microsoft Exchange контакта.
ms.openlocfilehash: 60bbcfb45e52dc92140d03cdd24a251ea84217b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465676"
---
# <a name="msexchangecertificate"></a><span data-ttu-id="37a0a-103">мсексчанжецертификате</span><span class="sxs-lookup"><span data-stu-id="37a0a-103">MSExchangeCertificate</span></span>

<span data-ttu-id="37a0a-104">Элемент **мсексчанжецертификате** содержит значение, которое кодирует сертификат Microsoft Exchange контакта.</span><span class="sxs-lookup"><span data-stu-id="37a0a-104">The **MSExchangeCertificate** element contains a value that encodes the Microsoft Exchange certificate of a contact.</span></span> 
  
```XML
<MSExchangeCertificate/>
```

 <span data-ttu-id="37a0a-105">**аррайофбинаритипе**</span><span class="sxs-lookup"><span data-stu-id="37a0a-105">**ArrayOfBinaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37a0a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="37a0a-106">Attributes and elements</span></span>

<span data-ttu-id="37a0a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="37a0a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37a0a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="37a0a-108">Attributes</span></span>

<span data-ttu-id="37a0a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="37a0a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37a0a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="37a0a-110">Child elements</span></span>

|<span data-ttu-id="37a0a-111">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="37a0a-111">**Element name**</span></span>|<span data-ttu-id="37a0a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37a0a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37a0a-113">Base64Binary</span><span class="sxs-lookup"><span data-stu-id="37a0a-113">Base64Binary</span></span>](base64binary.md) <br/> |<span data-ttu-id="37a0a-114">Содержит значение, закодированное в формате Base64.</span><span class="sxs-lookup"><span data-stu-id="37a0a-114">Contains a Base64-encoded value.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37a0a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="37a0a-115">Parent elements</span></span>

|<span data-ttu-id="37a0a-116">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="37a0a-116">**Element name**</span></span>|<span data-ttu-id="37a0a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37a0a-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="37a0a-118">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="37a0a-118">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="37a0a-119">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="37a0a-119">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="37a0a-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="37a0a-120">Text value</span></span>

<span data-ttu-id="37a0a-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="37a0a-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37a0a-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="37a0a-122">Remarks</span></span>

<span data-ttu-id="37a0a-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="37a0a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="37a0a-124">Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="37a0a-124">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37a0a-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="37a0a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37a0a-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="37a0a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="37a0a-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="37a0a-127">Schema name</span></span>  <br/> |<span data-ttu-id="37a0a-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="37a0a-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="37a0a-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="37a0a-129">Validation file</span></span>  <br/> |<span data-ttu-id="37a0a-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="37a0a-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="37a0a-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="37a0a-131">Can be empty</span></span>  <br/> |<span data-ttu-id="37a0a-132">False</span><span class="sxs-lookup"><span data-stu-id="37a0a-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37a0a-133">См. также</span><span class="sxs-lookup"><span data-stu-id="37a0a-133">See also</span></span>



- [<span data-ttu-id="37a0a-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37a0a-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="37a0a-135">Создание контактов (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="37a0a-135">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

