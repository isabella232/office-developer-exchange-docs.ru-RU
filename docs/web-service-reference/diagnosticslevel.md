---
title: DiagnosticsLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DiagnosticsLevel
api_type:
- schema
ms.assetid: 66794226-f5e0-44f0-8a0e-1f194bb0ba0f
description: Элемент DiagnosticsLevel представляет сведения о времени и производительности, который будет использоваться для формирования отчета.
ms.openlocfilehash: 9205625bb6cf38e370e29d96770eb293ed9277f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762088"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="881f8-103">DiagnosticsLevel</span><span class="sxs-lookup"><span data-stu-id="881f8-103">DiagnosticsLevel</span></span>

<span data-ttu-id="881f8-104">Элемент **DiagnosticsLevel** представляет сведения о времени и производительности, который будет использоваться для формирования отчета.</span><span class="sxs-lookup"><span data-stu-id="881f8-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="881f8-105">**string**</span><span class="sxs-lookup"><span data-stu-id="881f8-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="881f8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="881f8-106">Attributes and elements</span></span>

<span data-ttu-id="881f8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="881f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="881f8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="881f8-108">Attributes</span></span>

<span data-ttu-id="881f8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="881f8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="881f8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="881f8-110">Child elements</span></span>

<span data-ttu-id="881f8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="881f8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="881f8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="881f8-112">Parent elements</span></span>

|<span data-ttu-id="881f8-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="881f8-113">**Element**</span></span>|<span data-ttu-id="881f8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="881f8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="881f8-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="881f8-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="881f8-116">Содержит критерии для типов сообщений для поиска.</span><span class="sxs-lookup"><span data-stu-id="881f8-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="881f8-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="881f8-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="881f8-118">Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="881f8-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="881f8-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="881f8-119">Text value</span></span>

<span data-ttu-id="881f8-120">Текстовое значение, представляющее строку является обязательным, если данный элемент используется.</span><span class="sxs-lookup"><span data-stu-id="881f8-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="881f8-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="881f8-121">Remarks</span></span>

<span data-ttu-id="881f8-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="881f8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="881f8-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="881f8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="881f8-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="881f8-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="881f8-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="881f8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="881f8-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="881f8-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="881f8-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="881f8-127">Validation File</span></span>  <br/> |<span data-ttu-id="881f8-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="881f8-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="881f8-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="881f8-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="881f8-130">False</span><span class="sxs-lookup"><span data-stu-id="881f8-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="881f8-131">См. также</span><span class="sxs-lookup"><span data-stu-id="881f8-131">See also</span></span>

- [<span data-ttu-id="881f8-132">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="881f8-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="881f8-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="881f8-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

