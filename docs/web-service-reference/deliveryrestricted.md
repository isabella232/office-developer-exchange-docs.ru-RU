---
title: деливерирестриктед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryRestricted
api_type:
- schema
ms.assetid: 05989915-121c-4f26-93cc-af8d454ab442
description: Элемент Деливерирестриктед указывает, будут ли ограничения доставки допустить достижение получателем сообщения отправителя.
ms.openlocfilehash: 58fc85873326179d7745db4ba7d4854a76ced6a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462691"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="e238d-103">деливерирестриктед</span><span class="sxs-lookup"><span data-stu-id="e238d-103">DeliveryRestricted</span></span>

<span data-ttu-id="e238d-104">Элемент **деливерирестриктед** указывает, будут ли ограничения доставки допустить достижение получателем сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="e238d-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="e238d-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e238d-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e238d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e238d-106">Attributes and elements</span></span>

<span data-ttu-id="e238d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e238d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e238d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e238d-108">Attributes</span></span>

<span data-ttu-id="e238d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e238d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e238d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e238d-110">Child elements</span></span>

<span data-ttu-id="e238d-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e238d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e238d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e238d-112">Parent elements</span></span>

|<span data-ttu-id="e238d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e238d-113">**Element**</span></span>|<span data-ttu-id="e238d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e238d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e238d-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="e238d-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="e238d-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="e238d-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e238d-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e238d-117">Text value</span></span>

<span data-ttu-id="e238d-118">Текстовое значение этого элемента равно **true** , если ограничения доставки не допускают получателю сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="e238d-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="e238d-119">Значение **false** , если ограничения доставки не предотвращают достижение получателем сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="e238d-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e238d-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="e238d-120">Remarks</span></span>

<span data-ttu-id="e238d-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e238d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e238d-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e238d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e238d-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e238d-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e238d-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e238d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e238d-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e238d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e238d-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e238d-126">Validation File</span></span>  <br/> |<span data-ttu-id="e238d-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e238d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e238d-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e238d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e238d-129">False</span><span class="sxs-lookup"><span data-stu-id="e238d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e238d-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e238d-130">See also</span></span>

- [<span data-ttu-id="e238d-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e238d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

