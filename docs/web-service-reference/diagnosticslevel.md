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
ms.openlocfilehash: 3060d4f1b8449a5870d964bdfcdbf0d503905abc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467832"
---
# <a name="diagnosticslevel"></a><span data-ttu-id="b33f0-103">диагностикслевел</span><span class="sxs-lookup"><span data-stu-id="b33f0-103">DiagnosticsLevel</span></span>

<span data-ttu-id="b33f0-104">Элемент **диагностикслевел** представляет сведения о времени и производительности, которые будут использоваться для получения отчета.</span><span class="sxs-lookup"><span data-stu-id="b33f0-104">The **DiagnosticsLevel** element represents timing and performance information that will be used to derive the report.</span></span> 
  
```XML
<DiagnosticsLevel/>
```

 <span data-ttu-id="b33f0-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="b33f0-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b33f0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b33f0-106">Attributes and elements</span></span>

<span data-ttu-id="b33f0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b33f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b33f0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b33f0-108">Attributes</span></span>

<span data-ttu-id="b33f0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b33f0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b33f0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b33f0-110">Child elements</span></span>

<span data-ttu-id="b33f0-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b33f0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b33f0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b33f0-112">Parent elements</span></span>

|<span data-ttu-id="b33f0-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b33f0-113">**Element**</span></span>|<span data-ttu-id="b33f0-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b33f0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b33f0-115">FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b33f0-115">FindMessageTrackingReport</span></span>](findmessagetrackingreport.md) <br/> |<span data-ttu-id="b33f0-116">Содержит условия для типов сообщений, которые требуется найти.</span><span class="sxs-lookup"><span data-stu-id="b33f0-116">Contains criteria for the types of messages to find.</span></span>  <br/> |
|[<span data-ttu-id="b33f0-117">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b33f0-117">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="b33f0-118">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="b33f0-118">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b33f0-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b33f0-119">Text value</span></span>

<span data-ttu-id="b33f0-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="b33f0-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b33f0-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="b33f0-121">Remarks</span></span>

<span data-ttu-id="b33f0-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b33f0-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b33f0-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b33f0-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b33f0-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b33f0-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b33f0-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b33f0-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b33f0-126">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b33f0-126">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b33f0-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b33f0-127">Validation File</span></span>  <br/> |<span data-ttu-id="b33f0-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b33f0-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b33f0-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b33f0-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="b33f0-130">False</span><span class="sxs-lookup"><span data-stu-id="b33f0-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b33f0-131">См. также</span><span class="sxs-lookup"><span data-stu-id="b33f0-131">See also</span></span>

- [<span data-ttu-id="b33f0-132">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="b33f0-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="b33f0-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b33f0-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

