---
title: Диагностики
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Diagnostics
api_type:
- schema
ms.assetid: fecea440-970a-49da-9796-534ca470cbd6
description: Элемент Diagnostics предоставляет сведения о времени и производительности, которые используются для отчетов в центре обработки данных.
ms.openlocfilehash: 9eb46ef7ceb877372aff9b029190af8c8d8115cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467839"
---
# <a name="diagnostics"></a><span data-ttu-id="c1992-103">Диагностики</span><span class="sxs-lookup"><span data-stu-id="c1992-103">Diagnostics</span></span>

<span data-ttu-id="c1992-104">Элемент **Diagnostics** предоставляет сведения о времени и производительности, которые используются для отчетов в центре обработки данных.</span><span class="sxs-lookup"><span data-stu-id="c1992-104">The **Diagnostics** element provides timing and performance information that is used for reporting in a DataCenter.</span></span> 
  
```XML
<Diagnostics>
   <String/>
</Diagnostics>

```

 <span data-ttu-id="c1992-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="c1992-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1992-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1992-106">Attributes and elements</span></span>

<span data-ttu-id="c1992-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c1992-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1992-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1992-108">Attributes</span></span>

<span data-ttu-id="c1992-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c1992-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1992-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1992-110">Child elements</span></span>

|<span data-ttu-id="c1992-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1992-111">**Element**</span></span>|<span data-ttu-id="c1992-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1992-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1992-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c1992-113">String</span></span>](string.md) <br/> |<span data-ttu-id="c1992-114">Содержит строку, используемую элементами, контактами, задачами и беседами.</span><span class="sxs-lookup"><span data-stu-id="c1992-114">Contains a string that is used by items, contacts, tasks, and conversations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1992-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1992-115">Parent elements</span></span>

|<span data-ttu-id="c1992-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1992-116">**Element**</span></span>|<span data-ttu-id="c1992-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1992-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1992-118">финдмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="c1992-118">FindMessageTrackingReportResponse</span></span>](findmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="c1992-119">Содержит состояние и результат одного запроса [операции FindMessageTrackingReport](findmessagetrackingreport-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c1992-119">Contains the status and result of a single [FindMessageTrackingReport operation](findmessagetrackingreport-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="c1992-120">жетмессажетраккингрепортреспонсе</span><span class="sxs-lookup"><span data-stu-id="c1992-120">GetMessageTrackingReportResponse</span></span>](getmessagetrackingreportresponse.md) <br/> |<span data-ttu-id="c1992-121">Содержит ответ для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c1992-121">Contains the response for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md).</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c1992-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c1992-122">Text value</span></span>

<span data-ttu-id="c1992-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="c1992-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c1992-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="c1992-124">Remarks</span></span>

<span data-ttu-id="c1992-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c1992-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1992-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1992-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1992-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1992-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c1992-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1992-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c1992-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c1992-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c1992-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1992-130">Validation File</span></span>  <br/> |<span data-ttu-id="c1992-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c1992-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c1992-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1992-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1992-133">False</span><span class="sxs-lookup"><span data-stu-id="c1992-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1992-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c1992-134">See also</span></span>

- [<span data-ttu-id="c1992-135">Операция FindMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c1992-135">FindMessageTrackingReport operation</span></span>](findmessagetrackingreport-operation.md)
- [<span data-ttu-id="c1992-136">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="c1992-136">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)
- [<span data-ttu-id="c1992-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c1992-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

