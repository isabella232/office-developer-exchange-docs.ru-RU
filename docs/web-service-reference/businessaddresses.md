---
title: бусинессаддрессес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 828f8f62-7abf-44d4-8d58-f706d595a812
description: Элемент Бусинессаддрессес указывает массив бизнес-адресов и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: d314d0de679f8eabc51dc9ee3b2e9a57cd0b8da1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465928"
---
# <a name="businessaddresses"></a><span data-ttu-id="1143d-103">бусинессаддрессес</span><span class="sxs-lookup"><span data-stu-id="1143d-103">BusinessAddresses</span></span>

<span data-ttu-id="1143d-104">Элемент **бусинессаддрессес** указывает массив бизнес-адресов и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="1143d-104">The **BusinessAddresses** element specifies an array of business addresses and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<BusinessAddresses>
    <PostalAddressAttributedValue></PostalAddressAttributedValue>
</BusinessAddresses
```

 <span data-ttu-id="1143d-105">**аррайофпосталаддрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="1143d-105">**ArrayOfPostalAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1143d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1143d-106">Attributes and elements</span></span>

<span data-ttu-id="1143d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1143d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1143d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1143d-108">Attributes</span></span>

<span data-ttu-id="1143d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1143d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1143d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1143d-110">Child elements</span></span>

|<span data-ttu-id="1143d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1143d-111">**Element**</span></span>|<span data-ttu-id="1143d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1143d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1143d-113">посталаддрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="1143d-113">PostalAddressAttributedValue</span></span>](postaladdressattributedvalue.md) <br/> |<span data-ttu-id="1143d-114">Указывает экземпляр массива почтовых адресов и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="1143d-114">Specifies an instance of an array of postal addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1143d-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1143d-115">Parent elements</span></span>

|<span data-ttu-id="1143d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1143d-116">**Element**</span></span>|<span data-ttu-id="1143d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1143d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1143d-118">Роль</span><span class="sxs-lookup"><span data-stu-id="1143d-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="1143d-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="1143d-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1143d-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="1143d-120">Remarks</span></span>

<span data-ttu-id="1143d-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1143d-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1143d-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1143d-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1143d-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1143d-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1143d-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1143d-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1143d-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1143d-125">Schema Name</span></span>  <br/> |<span data-ttu-id="1143d-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="1143d-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="1143d-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1143d-127">Validation File</span></span>  <br/> |<span data-ttu-id="1143d-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="1143d-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1143d-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1143d-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="1143d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="1143d-130">See also</span></span>



- [<span data-ttu-id="1143d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1143d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

