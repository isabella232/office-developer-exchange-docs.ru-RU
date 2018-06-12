---
title: DeliveryRestricted
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
description: Элемент DeliveryRestricted указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762066"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="17c10-103">DeliveryRestricted</span><span class="sxs-lookup"><span data-stu-id="17c10-103">DeliveryRestricted</span></span>

<span data-ttu-id="17c10-104">Элемент **DeliveryRestricted** указывает ли ограничения на доставку будет препятствовать сообщения достигает получателя.</span><span class="sxs-lookup"><span data-stu-id="17c10-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="17c10-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="17c10-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17c10-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="17c10-106">Attributes and elements</span></span>

<span data-ttu-id="17c10-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="17c10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17c10-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="17c10-108">Attributes</span></span>

<span data-ttu-id="17c10-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="17c10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17c10-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="17c10-110">Child elements</span></span>

<span data-ttu-id="17c10-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="17c10-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17c10-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="17c10-112">Parent elements</span></span>

|<span data-ttu-id="17c10-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17c10-113">**Element**</span></span>|<span data-ttu-id="17c10-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17c10-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17c10-115">Почтовые подсказки</span><span class="sxs-lookup"><span data-stu-id="17c10-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="17c10-116">Представляет значения для различных типов почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="17c10-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17c10-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="17c10-117">Text value</span></span>

<span data-ttu-id="17c10-118">Текстовое значение этого элемента равно **true** , если ограничения на доставку будет препятствовать достигает получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="17c10-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="17c10-119">Значение равно **false** , если ограничения на доставку, не будет препятствовать достигает получателя сообщения.</span><span class="sxs-lookup"><span data-stu-id="17c10-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="17c10-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="17c10-120">Remarks</span></span>

<span data-ttu-id="17c10-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="17c10-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17c10-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="17c10-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17c10-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="17c10-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17c10-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="17c10-124">Schema Name</span></span>  <br/> |<span data-ttu-id="17c10-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="17c10-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="17c10-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="17c10-126">Validation File</span></span>  <br/> |<span data-ttu-id="17c10-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="17c10-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17c10-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="17c10-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="17c10-129">False</span><span class="sxs-lookup"><span data-stu-id="17c10-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17c10-130">См. также</span><span class="sxs-lookup"><span data-stu-id="17c10-130">See also</span></span>

- [<span data-ttu-id="17c10-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="17c10-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

