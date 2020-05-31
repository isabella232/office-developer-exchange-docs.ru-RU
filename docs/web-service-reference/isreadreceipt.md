---
title: исреадрецеипт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReadReceipt
api_type:
- schema
ms.assetid: e60e525f-c136-469a-b68b-b3dc01f400a6
description: Элемент Исреадрецеипт указывает, должны ли входящие сообщения принимать уведомления о прочтении для того, чтобы условие или исключение применялось.
ms.openlocfilehash: 78714aafb116a609a69d77b3b4f0fd15695bda34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834094"
---
# <a name="isreadreceipt"></a><span data-ttu-id="723dc-103">исреадрецеипт</span><span class="sxs-lookup"><span data-stu-id="723dc-103">IsReadReceipt</span></span>

<span data-ttu-id="723dc-104">Элемент **исреадрецеипт** указывает, должны ли входящие сообщения принимать уведомления о прочтении для того, чтобы условие или исключение применялось.</span><span class="sxs-lookup"><span data-stu-id="723dc-104">The **IsReadReceipt** element indicates whether incoming messages must be read receipts in order for the condition or exception to apply.</span></span> 
  
```XML
<IsReadReceipt> true | false</IsReadReceipt>
```

 <span data-ttu-id="723dc-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="723dc-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="723dc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="723dc-106">Attributes and elements</span></span>

<span data-ttu-id="723dc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="723dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="723dc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="723dc-108">Attributes</span></span>

<span data-ttu-id="723dc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="723dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="723dc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="723dc-110">Child elements</span></span>

<span data-ttu-id="723dc-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="723dc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="723dc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="723dc-112">Parent elements</span></span>

|<span data-ttu-id="723dc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="723dc-113">**Element**</span></span>|<span data-ttu-id="723dc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="723dc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="723dc-115">Условия</span><span class="sxs-lookup"><span data-stu-id="723dc-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="723dc-116">Представляет условия, если выполнены, запустит действия правил для этого правила.</span><span class="sxs-lookup"><span data-stu-id="723dc-116">Represents the conditions that, when fulfilled, will trigger the rule actions for that rule.</span></span>  <br/> |
|[<span data-ttu-id="723dc-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="723dc-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="723dc-118">Представляет доступных исключение условий для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="723dc-118">Represents all the available rule exception conditions for the Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="723dc-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="723dc-119">Text value</span></span>

<span data-ttu-id="723dc-120">Текстовое значение **true** указывает, что сообщение должно быть уведомлением о прочтении, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="723dc-120">A text value of **true** indicates that the message must be a read receipt in order for the condition or exception to apply.</span></span> <span data-ttu-id="723dc-121">Если сообщение не обязательно должно быть уведомлением о прочтении для условия или исключения, значение равно **false**.</span><span class="sxs-lookup"><span data-stu-id="723dc-121">If the message does not have to be a read receipt for the condition or exception to apply, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="723dc-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="723dc-122">Remarks</span></span>

<span data-ttu-id="723dc-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="723dc-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="723dc-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="723dc-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="723dc-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="723dc-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="723dc-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="723dc-126">Schema Name</span></span>  <br/> |<span data-ttu-id="723dc-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="723dc-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="723dc-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="723dc-128">Validation File</span></span>  <br/> |<span data-ttu-id="723dc-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="723dc-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="723dc-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="723dc-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="723dc-131">True</span><span class="sxs-lookup"><span data-stu-id="723dc-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="723dc-132">См. также</span><span class="sxs-lookup"><span data-stu-id="723dc-132">See also</span></span>



- [<span data-ttu-id="723dc-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="723dc-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

