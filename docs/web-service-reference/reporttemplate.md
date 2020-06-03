---
title: ReportTemplate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: Элемент ReportTemplate представляет тип получаемого отчета.
ms.openlocfilehash: 22f14d326032a30e5cb4c2c9e1aff390d98e95e0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528701"
---
# <a name="reporttemplate"></a><span data-ttu-id="5adcb-103">ReportTemplate</span><span class="sxs-lookup"><span data-stu-id="5adcb-103">ReportTemplate</span></span>

<span data-ttu-id="5adcb-104">Элемент **ReportTemplate** представляет тип получаемого отчета.</span><span class="sxs-lookup"><span data-stu-id="5adcb-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="5adcb-105">**мессажетраккингрепорттемплатетипе**</span><span class="sxs-lookup"><span data-stu-id="5adcb-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5adcb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5adcb-106">Attributes and elements</span></span>

<span data-ttu-id="5adcb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="5adcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5adcb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5adcb-108">Attributes</span></span>

<span data-ttu-id="5adcb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5adcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5adcb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5adcb-110">Child elements</span></span>

<span data-ttu-id="5adcb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5adcb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5adcb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5adcb-112">Parent elements</span></span>

|<span data-ttu-id="5adcb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5adcb-113">**Element**</span></span>|<span data-ttu-id="5adcb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5adcb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5adcb-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="5adcb-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="5adcb-116">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="5adcb-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5adcb-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5adcb-117">Text value</span></span>

<span data-ttu-id="5adcb-118">В следующей таблице приведены возможные значения для элемента **ReportTemplate** .</span><span class="sxs-lookup"><span data-stu-id="5adcb-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="5adcb-119">**Значения элементов ReportTemplate**</span><span class="sxs-lookup"><span data-stu-id="5adcb-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="5adcb-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="5adcb-120">**Value**</span></span>|<span data-ttu-id="5adcb-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5adcb-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5adcb-122">Сводка</span><span class="sxs-lookup"><span data-stu-id="5adcb-122">Summary</span></span>  <br/> |<span data-ttu-id="5adcb-123">Указывает, что в отчете будут отображаться все получатели сообщения и состояние доставки сообщения для каждого получателя.</span><span class="sxs-lookup"><span data-stu-id="5adcb-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="5adcb-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="5adcb-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="5adcb-125">Указывает, что для одного получателя в отчете будет отображаться полный журнал событий, которые произошли.</span><span class="sxs-lookup"><span data-stu-id="5adcb-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5adcb-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="5adcb-126">Remarks</span></span>

<span data-ttu-id="5adcb-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5adcb-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5adcb-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5adcb-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5adcb-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5adcb-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5adcb-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5adcb-130">Schema Name</span></span>  <br/> |<span data-ttu-id="5adcb-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5adcb-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5adcb-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5adcb-132">Validation File</span></span>  <br/> |<span data-ttu-id="5adcb-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5adcb-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5adcb-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5adcb-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="5adcb-135">False</span><span class="sxs-lookup"><span data-stu-id="5adcb-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5adcb-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5adcb-136">See also</span></span>



- [<span data-ttu-id="5adcb-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5adcb-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

