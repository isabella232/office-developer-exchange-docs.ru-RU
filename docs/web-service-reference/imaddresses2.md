---
title: ImAddresses2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 328f29b9-3a9c-4d9a-a85f-5ffff84e266a
description: Элемент ImAddresses2 указывает массив адресов обмена мгновенными сообщениями и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: f61084f22eb9d38766c45e63dfbacc0882ccaaca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833870"
---
# <a name="imaddresses2"></a><span data-ttu-id="95519-103">ImAddresses2</span><span class="sxs-lookup"><span data-stu-id="95519-103">ImAddresses2</span></span>

<span data-ttu-id="95519-104">Элемент **ImAddresses2** указывает массив адресов обмена мгновенными сообщениями и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="95519-104">The **ImAddresses2** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses2>
    <StringAttributedValue/>
</ImAddresses2>
```

 <span data-ttu-id="95519-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="95519-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95519-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="95519-106">Attributes and elements</span></span>

<span data-ttu-id="95519-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="95519-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95519-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="95519-108">Attributes</span></span>

<span data-ttu-id="95519-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="95519-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95519-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="95519-110">Child elements</span></span>

|<span data-ttu-id="95519-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95519-111">**Element**</span></span>|<span data-ttu-id="95519-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95519-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95519-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="95519-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="95519-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="95519-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95519-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="95519-115">Parent elements</span></span>

|<span data-ttu-id="95519-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="95519-116">**Element**</span></span>|<span data-ttu-id="95519-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="95519-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95519-118">Роль</span><span class="sxs-lookup"><span data-stu-id="95519-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="95519-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="95519-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95519-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="95519-120">Remarks</span></span>

<span data-ttu-id="95519-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="95519-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="95519-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="95519-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95519-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="95519-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95519-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="95519-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="95519-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="95519-125">Schema Name</span></span>  <br/> |<span data-ttu-id="95519-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="95519-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="95519-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="95519-127">Validation File</span></span>  <br/> |<span data-ttu-id="95519-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="95519-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="95519-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="95519-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="95519-130">См. также</span><span class="sxs-lookup"><span data-stu-id="95519-130">See also</span></span>



- [<span data-ttu-id="95519-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="95519-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

