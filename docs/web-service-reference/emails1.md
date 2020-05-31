---
title: Emails1
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cc02bd86-c618-446a-92f0-749423cbc4ee
description: Элемент Emails1 указывает массив значений Емаиладдрессаттрибутедвалуе и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: f1a1223244c91731b1a5a1beb9daed6d680d3bc4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762296"
---
# <a name="emails1"></a><span data-ttu-id="26cbd-103">Emails1</span><span class="sxs-lookup"><span data-stu-id="26cbd-103">Emails1</span></span>

<span data-ttu-id="26cbd-104">Элемент **Emails1** указывает массив значений **емаиладдрессаттрибутедвалуе** и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="26cbd-104">The **Emails1** element specifies an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails1>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails1>
```

 <span data-ttu-id="26cbd-105">**аррайофемаиладдрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="26cbd-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="26cbd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="26cbd-106">Attributes and elements</span></span>

<span data-ttu-id="26cbd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="26cbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="26cbd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="26cbd-108">Attributes</span></span>

<span data-ttu-id="26cbd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="26cbd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="26cbd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="26cbd-110">Child elements</span></span>

|<span data-ttu-id="26cbd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26cbd-111">**Element**</span></span>|<span data-ttu-id="26cbd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26cbd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26cbd-113">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="26cbd-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="26cbd-114">Указывает экземпляр массива адресов электронной почты и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="26cbd-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="26cbd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="26cbd-115">Parent elements</span></span>

|<span data-ttu-id="26cbd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="26cbd-116">**Element**</span></span>|<span data-ttu-id="26cbd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="26cbd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="26cbd-118">Роль</span><span class="sxs-lookup"><span data-stu-id="26cbd-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="26cbd-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="26cbd-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="26cbd-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="26cbd-120">Remarks</span></span>

<span data-ttu-id="26cbd-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="26cbd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="26cbd-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="26cbd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="26cbd-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="26cbd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="26cbd-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="26cbd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="26cbd-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="26cbd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="26cbd-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="26cbd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="26cbd-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="26cbd-127">Validation File</span></span>  <br/> |<span data-ttu-id="26cbd-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="26cbd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="26cbd-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="26cbd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="26cbd-130">См. также</span><span class="sxs-lookup"><span data-stu-id="26cbd-130">See also</span></span>



- [<span data-ttu-id="26cbd-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="26cbd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

