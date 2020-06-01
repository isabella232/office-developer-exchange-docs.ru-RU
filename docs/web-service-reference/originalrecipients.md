---
title: оригиналреЦипиентс
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
ms.openlocfilehash: 7385b1fd62313ee09c94cd04f3f669215e6cd497
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467181"
---
# <a name="originalrecipients"></a><span data-ttu-id="6f3ce-103">оригиналреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="6f3ce-103">OriginalRecipients</span></span>

<span data-ttu-id="6f3ce-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **OriginalRecipients** представляет список адресов электронной почты, первый получателей сообщения.</span><span class="sxs-lookup"><span data-stu-id="6f3ce-104">The **OriginalRecipients** element represents a list of e-mail addresses of the first message recipients.</span></span> 
  
```XML
<OriginalRecipients>
   <Address/>
</OriginalRecipients>
```

 <span data-ttu-id="6f3ce-105">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="6f3ce-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f3ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6f3ce-106">Attributes and elements</span></span>

<span data-ttu-id="6f3ce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6f3ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f3ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6f3ce-108">Attributes</span></span>

<span data-ttu-id="6f3ce-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6f3ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6f3ce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6f3ce-110">Child elements</span></span>

|<span data-ttu-id="6f3ce-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f3ce-111">**Element**</span></span>|<span data-ttu-id="6f3ce-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f3ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f3ce-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="6f3ce-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="6f3ce-114">Содержит адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="6f3ce-114">Contains a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6f3ce-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6f3ce-115">Parent elements</span></span>

|<span data-ttu-id="6f3ce-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6f3ce-116">**Element**</span></span>|<span data-ttu-id="6f3ce-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6f3ce-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f3ce-118">MessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6f3ce-118">MessageTrackingReport</span></span>](messagetrackingreport.md) <br/> |<span data-ttu-id="6f3ce-119">Содержит одно сообщение, которое возвращается в [Операция GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6f3ce-119">Contains a single message that is returned in a [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f3ce-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="6f3ce-120">Remarks</span></span>

<span data-ttu-id="6f3ce-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6f3ce-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f3ce-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6f3ce-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f3ce-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6f3ce-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f3ce-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6f3ce-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6f3ce-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6f3ce-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f3ce-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6f3ce-126">Validation File</span></span>  <br/> |<span data-ttu-id="6f3ce-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6f3ce-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f3ce-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6f3ce-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f3ce-129">False</span><span class="sxs-lookup"><span data-stu-id="6f3ce-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f3ce-130">См. также</span><span class="sxs-lookup"><span data-stu-id="6f3ce-130">See also</span></span>



[<span data-ttu-id="6f3ce-131">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="6f3ce-131">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="6f3ce-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6f3ce-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

