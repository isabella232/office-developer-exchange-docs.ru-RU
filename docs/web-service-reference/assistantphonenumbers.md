---
title: ассистантфоненумберс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd9ac1-7db3-44ea-9117-18488dddde15
description: Элемент Ассистантфоненумберс указывает массив телефонных номеров помощника и идентификаторы их исходных атрибутов для связанного пользователя.
ms.openlocfilehash: a72c8d646750b5d7cf9ebca13a51f4df84bf7bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464485"
---
# <a name="assistantphonenumbers"></a><span data-ttu-id="52a57-103">ассистантфоненумберс</span><span class="sxs-lookup"><span data-stu-id="52a57-103">AssistantPhoneNumbers</span></span>

<span data-ttu-id="52a57-104">Элемент **ассистантфоненумберс** указывает массив телефонных номеров помощника и идентификаторы их исходных атрибутов для связанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="52a57-104">The **AssistantPhoneNumbers** element specifies an array of assistant phone numbers and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<AssistantPhoneNumbers>
    <PhoneNumberAttributedValue></PhoneNumberAttributedValue>
</AssistantPhoneNumbers>
```

 <span data-ttu-id="52a57-105">**аррайоффоненумбераттрибутедвалуестипе**</span><span class="sxs-lookup"><span data-stu-id="52a57-105">**ArrayOfPhoneNumberAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="52a57-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="52a57-106">Attributes and elements</span></span>

<span data-ttu-id="52a57-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="52a57-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="52a57-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="52a57-108">Attributes</span></span>

<span data-ttu-id="52a57-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="52a57-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="52a57-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="52a57-110">Child elements</span></span>

|<span data-ttu-id="52a57-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52a57-111">**Element**</span></span>|<span data-ttu-id="52a57-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52a57-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52a57-113">фоненумбераттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="52a57-113">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md) <br/> |<span data-ttu-id="52a57-114">Указывает экземпляр массива номеров телефонов и связанные с ними атрибуты.</span><span class="sxs-lookup"><span data-stu-id="52a57-114">Specifies an instance of an array of phone numbers and their associated attributions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="52a57-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="52a57-115">Parent elements</span></span>

|<span data-ttu-id="52a57-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="52a57-116">**Element**</span></span>|<span data-ttu-id="52a57-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52a57-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52a57-118">Роль</span><span class="sxs-lookup"><span data-stu-id="52a57-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="52a57-119">Задает набор данных о пользователях, возвращаемых запросом к **другому человеку** .</span><span class="sxs-lookup"><span data-stu-id="52a57-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="52a57-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="52a57-120">Remarks</span></span>

<span data-ttu-id="52a57-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="52a57-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="52a57-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="52a57-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="52a57-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="52a57-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="52a57-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="52a57-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="52a57-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="52a57-125">Schema Name</span></span>  <br/> |<span data-ttu-id="52a57-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="52a57-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="52a57-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="52a57-127">Validation File</span></span>  <br/> |<span data-ttu-id="52a57-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="52a57-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="52a57-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="52a57-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="52a57-130">См. также</span><span class="sxs-lookup"><span data-stu-id="52a57-130">See also</span></span>

- [<span data-ttu-id="52a57-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="52a57-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

