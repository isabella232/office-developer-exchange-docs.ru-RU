---
title: OriginalRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OriginalRecipients
api_type:
- schema
ms.assetid: e4af86a5-85af-4239-8055-e29f0acf77c1
description: Элемент OriginalRecipients представляет список адресов электронной почты, первый получателей сообщения.
ms.openlocfilehash: 8f99368409dbfb5ac798b691be65c7fd64f32660
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834665"
---
# <a name="originalrecipients"></a><span data-ttu-id="e4c0b-103">OriginalRecipients</span><span class="sxs-lookup"><span data-stu-id="e4c0b-103">OriginalRecipients</span></span>

<span data-ttu-id="e4c0b-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **OriginalRecipients** представляет список адресов электронной почты, первый получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="e4c0b-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="e4c0b-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="e4c0b-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4c0b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4c0b-106">Attributes and elements</span></span>

<span data-ttu-id="e4c0b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e4c0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4c0b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4c0b-108">Attributes</span></span>

<span data-ttu-id="e4c0b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4c0b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4c0b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4c0b-110">Child elements</span></span>

|<span data-ttu-id="e4c0b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4c0b-111">**Element**</span></span>|<span data-ttu-id="e4c0b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4c0b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c0b-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e4c0b-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="e4c0b-114">Содержит адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="e4c0b-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e4c0b-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4c0b-115">Parent elements</span></span>

|<span data-ttu-id="e4c0b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4c0b-116">**Element**</span></span>|<span data-ttu-id="e4c0b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4c0b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c0b-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e4c0b-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="e4c0b-119">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e4c0b-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e4c0b-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="e4c0b-120">Remarks</span></span>

<span data-ttu-id="e4c0b-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4c0b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4c0b-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4c0b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4c0b-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4c0b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4c0b-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4c0b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e4c0b-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4c0b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4c0b-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4c0b-126">Validation File</span></span>  <br/> |<span data-ttu-id="e4c0b-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4c0b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4c0b-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4c0b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4c0b-129">False</span><span class="sxs-lookup"><span data-stu-id="e4c0b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4c0b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e4c0b-130">See also</span></span>



[<span data-ttu-id="e4c0b-131">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="e4c0b-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="e4c0b-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e4c0b-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

