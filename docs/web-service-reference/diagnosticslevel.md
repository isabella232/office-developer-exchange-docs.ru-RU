---
title: диагностикслевел
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
description: Элемент Диагностикслевел представляет сведения о времени и производительности, которые будут использоваться для получения отчета.
ms.openlocfilehash: 9205625bb6cf38e370e29d96770eb293ed9277f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762088"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="46115-103">диагностикслевел</span><span class="sxs-lookup"><span data-stu-id="46115-103">DiagnosticsLevel</span></span>

<span data-ttu-id="46115-104">Элемент **диагностикслевел** представляет сведения о времени и производительности, которые будут использоваться для получения отчета.</span><span class="sxs-lookup"><span data-stu-id="46115-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="46115-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="46115-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="46115-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46115-106">Attributes and elements</span></span>

<span data-ttu-id="46115-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="46115-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46115-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46115-108">Attributes</span></span>

<span data-ttu-id="46115-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="46115-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46115-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46115-110">Child elements</span></span>

<span data-ttu-id="46115-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="46115-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46115-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46115-112">Parent elements</span></span>

|<span data-ttu-id="46115-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="46115-113">**Element**</span></span>|<span data-ttu-id="46115-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="46115-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="46115-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="46115-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="46115-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="46115-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="46115-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="46115-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="46115-118">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="46115-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="46115-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="46115-119">Text value</span></span>

<span data-ttu-id="46115-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="46115-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="46115-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="46115-121">Remarks</span></span>

<span data-ttu-id="46115-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="46115-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46115-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46115-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46115-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46115-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="46115-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46115-125">Schema Name</span></span>  <br/> |<span data-ttu-id="46115-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="46115-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="46115-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46115-127">Validation File</span></span>  <br/> |<span data-ttu-id="46115-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="46115-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="46115-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46115-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="46115-130">False</span><span class="sxs-lookup"><span data-stu-id="46115-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46115-131">См. также</span><span class="sxs-lookup"><span data-stu-id="46115-131">See also</span></span>

- [<span data-ttu-id="46115-132">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="46115-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="46115-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46115-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

