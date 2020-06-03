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
ms.openlocfilehash: be756d86d7608fcb758dd54f2ada9f03a04343e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461200"
---
# <a name="fileas"></a><span data-ttu-id="5f352-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="5f352-103">FileAs</span></span>

<span data-ttu-id="5f352-104">Элемент **свойств fileas** представляет способ хранения контакта или списка рассылки в папке "Контакты".</span><span class="sxs-lookup"><span data-stu-id="5f352-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="5f352-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="5f352-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5f352-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5f352-106">Attributes and elements</span></span>

<span data-ttu-id="5f352-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5f352-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f352-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5f352-108">Attributes</span></span>

<span data-ttu-id="5f352-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5f352-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f352-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5f352-110">Child elements</span></span>

<span data-ttu-id="5f352-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5f352-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5f352-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5f352-112">Parent elements</span></span>

|<span data-ttu-id="5f352-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5f352-113">**Element**</span></span>|<span data-ttu-id="5f352-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5f352-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f352-115">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="5f352-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5f352-116">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="5f352-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5f352-117">Контакт</span><span class="sxs-lookup"><span data-stu-id="5f352-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5f352-118">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="5f352-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5f352-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5f352-119">Text value</span></span>

<span data-ttu-id="5f352-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="5f352-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5f352-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="5f352-121">Remarks</span></span>

<span data-ttu-id="5f352-122">Элемент **свойств fileas** используется для сортировки контактов и списков рассылки по имени, отличному от полного имени или названия компании.</span><span class="sxs-lookup"><span data-stu-id="5f352-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="5f352-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5f352-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5f352-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5f352-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5f352-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5f352-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5f352-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5f352-126">Schema name</span></span>  <br/> |<span data-ttu-id="5f352-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5f352-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="5f352-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5f352-128">Validation file</span></span>  <br/> |<span data-ttu-id="5f352-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="5f352-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5f352-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5f352-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5f352-131">False</span><span class="sxs-lookup"><span data-stu-id="5f352-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f352-132">См. также</span><span class="sxs-lookup"><span data-stu-id="5f352-132">See also</span></span>



- [<span data-ttu-id="5f352-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5f352-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

