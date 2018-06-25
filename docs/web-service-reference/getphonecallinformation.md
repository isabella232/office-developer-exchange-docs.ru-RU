---
title: GetPhoneCallInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformation
api_type:
- schema
ms.assetid: 5f4ee71c-bde0-4b0d-b426-0c24dfe67585
description: Элемент GetPhoneCallInformation определяет запрос на получение сведений о телефонный звонок.
ms.openlocfilehash: 2084a8b5e13b3fa03e0bf62439978bbe81d86ce9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762893"
---
# <a name="getphonecallinformation"></a><span data-ttu-id="c7a90-103">GetPhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="c7a90-103">GetPhoneCallInformation</span></span>

<span data-ttu-id="c7a90-104">Элемент **GetPhoneCallInformation** определяет запрос на получение сведений о телефонный звонок.</span><span class="sxs-lookup"><span data-stu-id="c7a90-104">The **GetPhoneCallInformation** element specifies a request to get telephone call information.</span></span> 
  
```xml
<GetPhoneCallInformation>
   <PhoneCallId/>
</GetPhoneCallInformation>
```

 <span data-ttu-id="c7a90-105">**GetPhoneCallInformationType**</span><span class="sxs-lookup"><span data-stu-id="c7a90-105">**GetPhoneCallInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7a90-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c7a90-106">Attributes and elements</span></span>

<span data-ttu-id="c7a90-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c7a90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7a90-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c7a90-108">Attributes</span></span>

<span data-ttu-id="c7a90-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7a90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7a90-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c7a90-110">Child elements</span></span>

|<span data-ttu-id="c7a90-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7a90-111">**Element**</span></span>|<span data-ttu-id="c7a90-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7a90-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7a90-113">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="c7a90-113">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="c7a90-114">Задает идентификатор телефонного звонка.</span><span class="sxs-lookup"><span data-stu-id="c7a90-114">Specifies the identifier of a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7a90-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c7a90-115">Parent elements</span></span>

<span data-ttu-id="c7a90-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7a90-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c7a90-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c7a90-117">Text value</span></span>

<span data-ttu-id="c7a90-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7a90-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c7a90-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="c7a90-119">Remarks</span></span>

<span data-ttu-id="c7a90-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7a90-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7a90-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c7a90-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7a90-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c7a90-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c7a90-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c7a90-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c7a90-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c7a90-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c7a90-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c7a90-125">Validation File</span></span>  <br/> |<span data-ttu-id="c7a90-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c7a90-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c7a90-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c7a90-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7a90-128">False</span><span class="sxs-lookup"><span data-stu-id="c7a90-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7a90-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c7a90-129">See also</span></span>



- [<span data-ttu-id="c7a90-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7a90-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

