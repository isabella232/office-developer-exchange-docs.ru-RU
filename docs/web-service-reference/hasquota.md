---
title: хаскуота
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasQuota
api_type:
- schema
ms.assetid: b6e4fef0-92a9-415f-81ae-0c5ecb7c12ad
description: Элемент Хаскуота указывает, есть ли у управляемой папки квота.
ms.openlocfilehash: 6e32aa4c69943774be928339936cca5016c58d85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462754"
---
# <a name="hasquota"></a><span data-ttu-id="f982c-103">хаскуота</span><span class="sxs-lookup"><span data-stu-id="f982c-103">HasQuota</span></span>

<span data-ttu-id="f982c-104">Элемент **хаскуота** указывает, есть ли у управляемой папки квота.</span><span class="sxs-lookup"><span data-stu-id="f982c-104">The **HasQuota** element indicates whether the managed folder has a quota.</span></span> 
  
```xml
<HasQuota/>
```

 <span data-ttu-id="f982c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f982c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f982c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f982c-106">Attributes and elements</span></span>

<span data-ttu-id="f982c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f982c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f982c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f982c-108">Attributes</span></span>

<span data-ttu-id="f982c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f982c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f982c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f982c-110">Child elements</span></span>

<span data-ttu-id="f982c-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f982c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f982c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f982c-112">Parent elements</span></span>

|<span data-ttu-id="f982c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f982c-113">**Element**</span></span>|<span data-ttu-id="f982c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f982c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f982c-115">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="f982c-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="f982c-116">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="f982c-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f982c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f982c-117">Text value</span></span>

<span data-ttu-id="f982c-118">Текстовое значение представляет логическое значение.</span><span class="sxs-lookup"><span data-stu-id="f982c-118">The text value represents a Boolean value.</span></span> <span data-ttu-id="f982c-119">Значение **true** указывает, что папка имеет квоту; значение **false** указывает, что у папки нет квоты.</span><span class="sxs-lookup"><span data-stu-id="f982c-119">A value of **true** indicates that the folder has a quota; a value of **false** indicates that the folder does not have a quota.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f982c-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="f982c-120">Remarks</span></span>

<span data-ttu-id="f982c-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f982c-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f982c-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f982c-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f982c-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f982c-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f982c-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f982c-124">Schema name</span></span>  <br/> |<span data-ttu-id="f982c-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f982c-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="f982c-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f982c-126">Validation file</span></span>  <br/> |<span data-ttu-id="f982c-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f982c-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f982c-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f982c-128">Can be empty</span></span>  <br/> |<span data-ttu-id="f982c-129">False</span><span class="sxs-lookup"><span data-stu-id="f982c-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f982c-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f982c-130">See also</span></span>



- [<span data-ttu-id="f982c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f982c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

