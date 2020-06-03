---
title: Получатели (АррайофреЦипиентстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: f4b71403-cbae-4176-8b2e-3597048c057b
description: Элемент Recipients представляет коллекцию получателей, которые получают копию сообщения.
ms.openlocfilehash: 0e18152a8143b888ad27f48137c06613694f5713
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463876"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="31be6-103">Получатели (АррайофреЦипиентстипе)</span><span class="sxs-lookup"><span data-stu-id="31be6-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="31be6-104">Элемент **Recipients** представляет коллекцию получателей, которые получают копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="31be6-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="31be6-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="31be6-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="31be6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="31be6-106">Attributes and elements</span></span>

<span data-ttu-id="31be6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="31be6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="31be6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="31be6-108">Attributes</span></span>

<span data-ttu-id="31be6-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="31be6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="31be6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="31be6-110">Child elements</span></span>

|<span data-ttu-id="31be6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31be6-111">**Element**</span></span>|<span data-ttu-id="31be6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31be6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31be6-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="31be6-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="31be6-114">Определяет объект Active Directory с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="31be6-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="31be6-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="31be6-115">Parent elements</span></span>

|<span data-ttu-id="31be6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="31be6-116">**Element**</span></span>|<span data-ttu-id="31be6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="31be6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="31be6-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="31be6-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="31be6-119">Содержит получателей и типы советов по работе с почтой, которые необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="31be6-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="31be6-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="31be6-120">Text value</span></span>

<span data-ttu-id="31be6-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="31be6-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="31be6-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="31be6-122">Remarks</span></span>

<span data-ttu-id="31be6-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="31be6-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="31be6-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="31be6-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="31be6-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="31be6-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="31be6-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="31be6-126">Schema Name</span></span>  <br/> |<span data-ttu-id="31be6-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="31be6-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="31be6-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="31be6-128">Validation File</span></span>  <br/> |<span data-ttu-id="31be6-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="31be6-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="31be6-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="31be6-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="31be6-131">False</span><span class="sxs-lookup"><span data-stu-id="31be6-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="31be6-132">См. также</span><span class="sxs-lookup"><span data-stu-id="31be6-132">See also</span></span>



- [<span data-ttu-id="31be6-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="31be6-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

