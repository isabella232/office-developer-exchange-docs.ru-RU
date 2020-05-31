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
ms.openlocfilehash: ba1c6e00b93c9e442a427fe98a5e15bf5fe1effd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762066"
---
# <a name="deliveryrestricted"></a><span data-ttu-id="99472-103">деливерирестриктед</span><span class="sxs-lookup"><span data-stu-id="99472-103">DeliveryRestricted</span></span>

<span data-ttu-id="99472-104">Элемент **деливерирестриктед** указывает, будут ли ограничения доставки допустить достижение получателем сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="99472-104">The **DeliveryRestricted** element indicates whether delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> 
  
```XML
<DeliveryRestricted>true | false</DeliveryRestricted>
```

 <span data-ttu-id="99472-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="99472-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="99472-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="99472-106">Attributes and elements</span></span>

<span data-ttu-id="99472-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="99472-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99472-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="99472-108">Attributes</span></span>

<span data-ttu-id="99472-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="99472-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="99472-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="99472-110">Child elements</span></span>

<span data-ttu-id="99472-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="99472-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="99472-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="99472-112">Parent elements</span></span>

|<span data-ttu-id="99472-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="99472-113">**Element**</span></span>|<span data-ttu-id="99472-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="99472-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99472-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="99472-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="99472-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="99472-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="99472-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="99472-117">Text value</span></span>

<span data-ttu-id="99472-118">Текстовое значение этого элемента равно **true** , если ограничения доставки не допускают получателю сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="99472-118">The text value of this element is **true** if delivery restrictions will prevent the sender's message from reaching the recipient.</span></span> <span data-ttu-id="99472-119">Значение **false** , если ограничения доставки не предотвращают достижение получателем сообщения отправителя.</span><span class="sxs-lookup"><span data-stu-id="99472-119">The value is **false** if delivery restrictions will not prevent the sender's message from reaching the recipient.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="99472-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="99472-120">Remarks</span></span>

<span data-ttu-id="99472-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="99472-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="99472-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="99472-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="99472-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="99472-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="99472-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="99472-124">Schema Name</span></span>  <br/> |<span data-ttu-id="99472-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="99472-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="99472-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="99472-126">Validation File</span></span>  <br/> |<span data-ttu-id="99472-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="99472-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="99472-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="99472-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="99472-129">False</span><span class="sxs-lookup"><span data-stu-id="99472-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99472-130">См. также</span><span class="sxs-lookup"><span data-stu-id="99472-130">See also</span></span>

- [<span data-ttu-id="99472-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="99472-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

