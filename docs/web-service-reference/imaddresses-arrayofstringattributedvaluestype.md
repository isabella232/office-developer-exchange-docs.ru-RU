---
title: Адреса (Аррайофстрингаттрибутедвалуестипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b95d0a8b-15a6-4711-b014-55698dbd679c
description: Элемент Addressing указывает массив адресов обмена мгновенными сообщениями и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: 6714af5d88e50047f48da2f10dbb33d2e2feb724
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460444"
---
# <a name="imaddresses-arrayofstringattributedvaluestype"></a><span data-ttu-id="4d594-103">Адреса (Аррайофстрингаттрибутедвалуестипе)</span><span class="sxs-lookup"><span data-stu-id="4d594-103">ImAddresses (ArrayOfStringAttributedValuesType)</span></span>

<span data-ttu-id="4d594-104">Элемент **Addressing** указывает массив адресов обмена мгновенными сообщениями и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d594-104">The **ImAddresses** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses>
    <StringAttributedValue/>
</ImAddresses>
```

 <span data-ttu-id="4d594-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="4d594-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d594-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d594-106">Attributes and elements</span></span>

<span data-ttu-id="4d594-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4d594-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d594-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d594-108">Attributes</span></span>

<span data-ttu-id="4d594-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d594-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d594-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d594-110">Child elements</span></span>

|<span data-ttu-id="4d594-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d594-111">**Element**</span></span>|<span data-ttu-id="4d594-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d594-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d594-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="4d594-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="4d594-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="4d594-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d594-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d594-115">Parent elements</span></span>

|<span data-ttu-id="4d594-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d594-116">**Element**</span></span>|<span data-ttu-id="4d594-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d594-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d594-118">Роль</span><span class="sxs-lookup"><span data-stu-id="4d594-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="4d594-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="4d594-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d594-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4d594-120">Remarks</span></span>

<span data-ttu-id="4d594-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4d594-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4d594-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4d594-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d594-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d594-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d594-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d594-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d594-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d594-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4d594-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4d594-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4d594-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d594-127">Validation File</span></span>  <br/> |<span data-ttu-id="4d594-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4d594-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d594-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d594-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4d594-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4d594-130">See also</span></span>



- [<span data-ttu-id="4d594-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d594-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

