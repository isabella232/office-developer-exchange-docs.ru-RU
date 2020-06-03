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
ms.openlocfilehash: b2a9f61ba31c1324ac5563bb6ab6b30f0271c653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460766"
---
# <a name="imaddresses2"></a><span data-ttu-id="47405-103">ImAddresses2</span><span class="sxs-lookup"><span data-stu-id="47405-103">ImAddresses2</span></span>

<span data-ttu-id="47405-104">Элемент **ImAddresses2** указывает массив адресов обмена мгновенными сообщениями и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="47405-104">The **ImAddresses2** element specifies an array of instant message addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<ImAddresses2>
    <StringAttributedValue/>
</ImAddresses2>
```

 <span data-ttu-id="47405-105">**аррайофстрингаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="47405-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="47405-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="47405-106">Attributes and elements</span></span>

<span data-ttu-id="47405-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="47405-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="47405-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="47405-108">Attributes</span></span>

<span data-ttu-id="47405-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="47405-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="47405-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="47405-110">Child elements</span></span>

|<span data-ttu-id="47405-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="47405-111">**Element**</span></span>|<span data-ttu-id="47405-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="47405-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47405-113">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="47405-113">StringAttributedValue</span></span>](stringattributedvalue.md) <br/> |<span data-ttu-id="47405-114">Указывает экземпляр в массиве атрибутов, связанных с элементом персоны.</span><span class="sxs-lookup"><span data-stu-id="47405-114">Specifies an instance in an array of attributes associated with a persona element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="47405-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="47405-115">Parent elements</span></span>

|<span data-ttu-id="47405-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="47405-116">**Element**</span></span>|<span data-ttu-id="47405-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="47405-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="47405-118">Роль</span><span class="sxs-lookup"><span data-stu-id="47405-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="47405-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="47405-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="47405-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="47405-120">Remarks</span></span>

<span data-ttu-id="47405-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="47405-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="47405-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="47405-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="47405-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="47405-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="47405-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="47405-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="47405-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="47405-125">Schema Name</span></span>  <br/> |<span data-ttu-id="47405-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="47405-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="47405-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="47405-127">Validation File</span></span>  <br/> |<span data-ttu-id="47405-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="47405-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="47405-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="47405-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="47405-130">См. также</span><span class="sxs-lookup"><span data-stu-id="47405-130">See also</span></span>



- [<span data-ttu-id="47405-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="47405-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

