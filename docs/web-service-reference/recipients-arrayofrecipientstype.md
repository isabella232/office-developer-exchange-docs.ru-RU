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
ms.openlocfilehash: b24a029bfacd6cc40e85a201b8ca90efd7790e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834991"
---
# <a name="recipients-arrayofrecipientstype"></a><span data-ttu-id="4a1a4-103">Получатели (АррайофреЦипиентстипе)</span><span class="sxs-lookup"><span data-stu-id="4a1a4-103">Recipients (ArrayOfRecipientsType)</span></span>

<span data-ttu-id="4a1a4-104">Элемент **Recipients** представляет коллекцию получателей, которые получают копию сообщения.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-104">The **Recipients** element represents a collection of recipients that receive a copy of the message.</span></span> 
  
```XML
<Recipients>
   <Mailbox/>
</Recipients>
```

 <span data-ttu-id="4a1a4-105">**аррайофреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="4a1a4-105">**ArrayOfRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a1a4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4a1a4-106">Attributes and elements</span></span>

<span data-ttu-id="4a1a4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a1a4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4a1a4-108">Attributes</span></span>

<span data-ttu-id="4a1a4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a1a4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4a1a4-110">Child elements</span></span>

|<span data-ttu-id="4a1a4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a1a4-111">**Element**</span></span>|<span data-ttu-id="4a1a4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a1a4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a1a4-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4a1a4-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="4a1a4-114">Определяет объект Active Directory с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-114">Identifies a mail-enabled Active Directory object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a1a4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4a1a4-115">Parent elements</span></span>

|<span data-ttu-id="4a1a4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4a1a4-116">**Element**</span></span>|<span data-ttu-id="4a1a4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4a1a4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a1a4-118">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="4a1a4-118">GetMailTips</span></span>](getmailtips.md) <br/> |<span data-ttu-id="4a1a4-119">Содержит получателей и типы советов по работе с почтой, которые необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-119">Contains the recipients and types of mail tips to retrieve.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a1a4-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4a1a4-120">Text value</span></span>

<span data-ttu-id="4a1a4-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a1a4-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="4a1a4-122">Remarks</span></span>

<span data-ttu-id="4a1a4-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4a1a4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a1a4-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4a1a4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a1a4-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4a1a4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a1a4-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4a1a4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4a1a4-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4a1a4-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a1a4-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4a1a4-128">Validation File</span></span>  <br/> |<span data-ttu-id="4a1a4-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4a1a4-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a1a4-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4a1a4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a1a4-131">False</span><span class="sxs-lookup"><span data-stu-id="4a1a4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a1a4-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4a1a4-132">See also</span></span>



- [<span data-ttu-id="4a1a4-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4a1a4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

