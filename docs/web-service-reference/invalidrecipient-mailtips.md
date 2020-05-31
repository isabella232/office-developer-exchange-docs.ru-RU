---
title: ИнвалидреЦипиент (подсказки)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: Элемент ИнвалидреЦипиент указывает, является ли получатель недопустимым.
ms.openlocfilehash: addb86ece2be3091ac55a52ee2f16f5c5f72ae41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833958"
---
# <a name="invalidrecipient-mailtips"></a><span data-ttu-id="c4140-103">ИнвалидреЦипиент (подсказки)</span><span class="sxs-lookup"><span data-stu-id="c4140-103">InvalidRecipient (MailTips)</span></span>

<span data-ttu-id="c4140-104">Элемент **инвалидреЦипиент** указывает, является ли получатель недопустимым.</span><span class="sxs-lookup"><span data-stu-id="c4140-104">The **InvalidRecipient** element indicates whether the recipient is invalid.</span></span> 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
```

 <span data-ttu-id="c4140-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c4140-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4140-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c4140-106">Attributes and elements</span></span>

<span data-ttu-id="c4140-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c4140-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4140-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c4140-108">Attributes</span></span>

<span data-ttu-id="c4140-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4140-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4140-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c4140-110">Child elements</span></span>

<span data-ttu-id="c4140-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4140-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4140-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c4140-112">Parent elements</span></span>

|<span data-ttu-id="c4140-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c4140-113">**Element**</span></span>|<span data-ttu-id="c4140-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4140-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4140-115">Подсказки</span><span class="sxs-lookup"><span data-stu-id="c4140-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="c4140-116">Представляет значения для различных типов советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c4140-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c4140-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c4140-117">Text value</span></span>

<span data-ttu-id="c4140-118">Текстовое значение этого элемента равно **true** , если получатель не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="c4140-118">The text value of this element is **true** if the recipient is invalid.</span></span> <span data-ttu-id="c4140-119">Значение **false** , если получатель не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="c4140-119">The value is **false** if the recipient is not invalid.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c4140-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="c4140-120">Remarks</span></span>

<span data-ttu-id="c4140-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4140-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4140-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c4140-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4140-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c4140-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4140-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c4140-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c4140-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c4140-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4140-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c4140-126">Validation File</span></span>  <br/> |<span data-ttu-id="c4140-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c4140-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4140-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c4140-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4140-129">False</span><span class="sxs-lookup"><span data-stu-id="c4140-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4140-130">См. также</span><span class="sxs-lookup"><span data-stu-id="c4140-130">See also</span></span>



- [<span data-ttu-id="c4140-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c4140-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

