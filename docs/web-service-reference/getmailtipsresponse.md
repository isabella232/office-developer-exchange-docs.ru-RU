---
title: жетмаилтипсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTipsResponse
api_type:
- schema
ms.assetid: fe270e34-566e-4f9e-9e73-fbf38e06436d
description: Элемент Жетмаилтипсреспонсе представляет ответное сообщение для операции с помощью вложенных подсказок.
ms.openlocfilehash: 2c0dcfe4e2deddcf9a6f4bb9d68d59115c171796
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458609"
---
# <a name="getmailtipsresponse"></a><span data-ttu-id="b59ed-103">жетмаилтипсреспонсе</span><span class="sxs-lookup"><span data-stu-id="b59ed-103">GetMailTipsResponse</span></span>

<span data-ttu-id="b59ed-104">Элемент **жетмаилтипсреспонсе** представляет ответное сообщение для операции с помощью вложенных [подсказок](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b59ed-104">The **GetMailTipsResponse** element represents the response message for a [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<GetMailTipsResponse>
   <ResponseMessages/>
</GetMailTipsResponse>
```

 <span data-ttu-id="b59ed-105">**жетмаилтипсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="b59ed-105">**GetMailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b59ed-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b59ed-106">Attributes and elements</span></span>

<span data-ttu-id="b59ed-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b59ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b59ed-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b59ed-108">Attributes</span></span>

<span data-ttu-id="b59ed-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b59ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b59ed-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b59ed-110">Child elements</span></span>

|<span data-ttu-id="b59ed-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b59ed-111">**Element**</span></span>|<span data-ttu-id="b59ed-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b59ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b59ed-113">Респонсемессажес (Аррайофмаилтипсреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="b59ed-113">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="b59ed-114">Представляет список ответных сообщений с советами по почте.</span><span class="sxs-lookup"><span data-stu-id="b59ed-114">Represents a list of mail tips response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b59ed-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b59ed-115">Parent elements</span></span>

<span data-ttu-id="b59ed-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b59ed-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b59ed-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b59ed-117">Text value</span></span>

<span data-ttu-id="b59ed-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="b59ed-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b59ed-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="b59ed-119">Remarks</span></span>

<span data-ttu-id="b59ed-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b59ed-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b59ed-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b59ed-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b59ed-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b59ed-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b59ed-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b59ed-123">Schema Name</span></span>  <br/> |<span data-ttu-id="b59ed-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b59ed-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b59ed-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b59ed-125">Validation File</span></span>  <br/> |<span data-ttu-id="b59ed-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b59ed-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b59ed-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b59ed-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="b59ed-128">False</span><span class="sxs-lookup"><span data-stu-id="b59ed-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b59ed-129">См. также</span><span class="sxs-lookup"><span data-stu-id="b59ed-129">See also</span></span>



[<span data-ttu-id="b59ed-130">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="b59ed-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="b59ed-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b59ed-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

