---
title: шовекстерналреЦипиенткаунт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Элемент ШовекстерналреЦипиенткаунт указывает, должны ли потребители операции с подсказками показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460472"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="84309-103">шовекстерналреЦипиенткаунт</span><span class="sxs-lookup"><span data-stu-id="84309-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="84309-104">Элемент **шовекстерналреЦипиенткаунт** указывает, должны ли потребители [операции](getmailtips-operation.md) с подсказками показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="84309-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="84309-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="84309-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84309-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="84309-106">Attributes and elements</span></span>

<span data-ttu-id="84309-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="84309-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84309-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="84309-108">Attributes</span></span>

<span data-ttu-id="84309-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84309-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84309-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="84309-110">Child elements</span></span>

<span data-ttu-id="84309-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="84309-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84309-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="84309-112">Parent elements</span></span>

|<span data-ttu-id="84309-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="84309-113">**Element**</span></span>|<span data-ttu-id="84309-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="84309-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84309-115">Маилтипсконфигуратион (Маилтипссервицеконфигуратион)</span><span class="sxs-lookup"><span data-stu-id="84309-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="84309-116">Содержит сведения о конфигурации службы для советов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="84309-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84309-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="84309-117">Text value</span></span>

<span data-ttu-id="84309-118">Текстовое значение этого элемента имеет значение **true** , если потребители [операции](getmailtips-operation.md) с подсказками должны отображать подсказки для почты, указывающие количество внешних получателей, на которые адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="84309-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="84309-119">Значение **false** , если потребители [операции](getmailtips-operation.md) с подсказками не должны показывать подсказки, указывающие количество внешних получателей, на которые адресовано сообщение.</span><span class="sxs-lookup"><span data-stu-id="84309-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="84309-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="84309-120">Remarks</span></span>

<span data-ttu-id="84309-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="84309-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84309-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="84309-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84309-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="84309-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84309-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="84309-124">Schema Name</span></span>  <br/> |<span data-ttu-id="84309-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="84309-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="84309-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="84309-126">Validation File</span></span>  <br/> |<span data-ttu-id="84309-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="84309-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84309-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="84309-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="84309-129">False</span><span class="sxs-lookup"><span data-stu-id="84309-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84309-130">См. также</span><span class="sxs-lookup"><span data-stu-id="84309-130">See also</span></span>



[<span data-ttu-id="84309-131">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="84309-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="84309-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="84309-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

