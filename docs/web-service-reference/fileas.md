---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: Элемент свойств fileas представляет способ хранения контакта или списка рассылки в папке "Контакты".
ms.openlocfilehash: dab9142eebf7691862e7970a7d1e8f5874393b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762539"
---
# <a name="fileas"></a><span data-ttu-id="c0f70-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="c0f70-103">FileAs</span></span>

<span data-ttu-id="c0f70-104">Элемент **свойств fileas** представляет способ хранения контакта или списка рассылки в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="c0f70-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="c0f70-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="c0f70-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0f70-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c0f70-106">Attributes and elements</span></span>

<span data-ttu-id="c0f70-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c0f70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0f70-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c0f70-108">Attributes</span></span>

<span data-ttu-id="c0f70-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0f70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0f70-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c0f70-110">Child elements</span></span>

<span data-ttu-id="c0f70-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0f70-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0f70-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c0f70-112">Parent elements</span></span>

|<span data-ttu-id="c0f70-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c0f70-113">**Element**</span></span>|<span data-ttu-id="c0f70-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0f70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0f70-115">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="c0f70-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="c0f70-116">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="c0f70-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c0f70-117">Контакт</span><span class="sxs-lookup"><span data-stu-id="c0f70-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="c0f70-118">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0f70-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c0f70-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c0f70-119">Text value</span></span>

<span data-ttu-id="c0f70-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="c0f70-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c0f70-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="c0f70-121">Remarks</span></span>

<span data-ttu-id="c0f70-122">Элемент **свойств fileas** используется для сортировки контактов и списков рассылки по имени, отличному от полного имени или названия компании.</span><span class="sxs-lookup"><span data-stu-id="c0f70-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="c0f70-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c0f70-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0f70-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c0f70-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0f70-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c0f70-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0f70-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c0f70-126">Schema name</span></span>  <br/> |<span data-ttu-id="c0f70-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c0f70-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0f70-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c0f70-128">Validation file</span></span>  <br/> |<span data-ttu-id="c0f70-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c0f70-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0f70-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c0f70-130">Can be empty</span></span>  <br/> |<span data-ttu-id="c0f70-131">False</span><span class="sxs-lookup"><span data-stu-id="c0f70-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0f70-132">См. также</span><span class="sxs-lookup"><span data-stu-id="c0f70-132">See also</span></span>



- [<span data-ttu-id="c0f70-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c0f70-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

