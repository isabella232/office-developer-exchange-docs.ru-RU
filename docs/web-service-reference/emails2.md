---
title: Emails2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6ad95936-f61b-431a-9d86-df160b5d4b2d
description: Элемент Emails2 содержит массив значений Емаиладдрессаттрибутедвалуе и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: b9445dfdc556ade1ad96d6e56c35ec1e56627e8c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463414"
---
# <a name="emails2"></a><span data-ttu-id="49a41-103">Emails2</span><span class="sxs-lookup"><span data-stu-id="49a41-103">Emails2</span></span>

<span data-ttu-id="49a41-104">Элемент **Emails2** содержит массив значений **емаиладдрессаттрибутедвалуе** и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="49a41-104">The **Emails2** element contains an array of **EmailAddressAttributedValue** values and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<Emails2>
    <EmailAddressAttributedValue></EmailAddressAttributedValue>
</Emails2>
```

 <span data-ttu-id="49a41-105">**аррайофемаиладдрессаттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="49a41-105">**ArrayOfEmailAddressAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49a41-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49a41-106">Attributes and elements</span></span>

<span data-ttu-id="49a41-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="49a41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49a41-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49a41-108">Attributes</span></span>

<span data-ttu-id="49a41-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49a41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49a41-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49a41-110">Child elements</span></span>

|<span data-ttu-id="49a41-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49a41-111">**Element**</span></span>|<span data-ttu-id="49a41-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49a41-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49a41-113">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="49a41-113">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md) <br/> |<span data-ttu-id="49a41-114">Указывает экземпляр массива адресов электронной почты и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="49a41-114">Specifies an instance of an array of email addresses and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49a41-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49a41-115">Parent elements</span></span>

|<span data-ttu-id="49a41-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49a41-116">**Element**</span></span>|<span data-ttu-id="49a41-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49a41-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49a41-118">Роль</span><span class="sxs-lookup"><span data-stu-id="49a41-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="49a41-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="49a41-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49a41-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="49a41-120">Remarks</span></span>

<span data-ttu-id="49a41-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="49a41-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="49a41-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="49a41-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49a41-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49a41-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49a41-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49a41-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49a41-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49a41-125">Schema Name</span></span>  <br/> |<span data-ttu-id="49a41-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="49a41-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="49a41-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49a41-127">Validation File</span></span>  <br/> |<span data-ttu-id="49a41-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="49a41-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="49a41-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49a41-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="49a41-130">См. также</span><span class="sxs-lookup"><span data-stu-id="49a41-130">See also</span></span>



- [<span data-ttu-id="49a41-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="49a41-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

