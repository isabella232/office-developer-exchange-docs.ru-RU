---
title: Шаблон_отчета
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
description: Элемент Шаблон_отчета представляет тип отчета требуется получить.
ms.openlocfilehash: 70aab69f4d20ad9fd7e878c7fccd16e261c9b94c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835118"
---
# <a name="reporttemplate"></a><span data-ttu-id="a5047-103">Шаблон_отчета</span><span class="sxs-lookup"><span data-stu-id="a5047-103">ReportTemplate</span></span>

<span data-ttu-id="a5047-104">Элемент **Шаблон_отчета** представляет тип отчета требуется получить.</span><span class="sxs-lookup"><span data-stu-id="a5047-104">The **ReportTemplate** element represents the type of report to get.</span></span> 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 <span data-ttu-id="a5047-105">**MessageTrackingReportTemplateType**</span><span class="sxs-lookup"><span data-stu-id="a5047-105">**MessageTrackingReportTemplateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a5047-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a5047-106">Attributes and elements</span></span>

<span data-ttu-id="a5047-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a5047-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a5047-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a5047-108">Attributes</span></span>

<span data-ttu-id="a5047-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5047-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a5047-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a5047-110">Child elements</span></span>

<span data-ttu-id="a5047-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a5047-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a5047-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a5047-112">Parent elements</span></span>

|<span data-ttu-id="a5047-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a5047-113">**Element**</span></span>|<span data-ttu-id="a5047-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5047-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a5047-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="a5047-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="a5047-116">Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="a5047-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a5047-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a5047-117">Text value</span></span>

<span data-ttu-id="a5047-118">В следующей таблице приведены возможные значения для элемента **Шаблон_отчета** .</span><span class="sxs-lookup"><span data-stu-id="a5047-118">The following table lists the possible values for the **ReportTemplate** element.</span></span> 
  
<span data-ttu-id="a5047-119">**Значения элементов Шаблон_отчета**</span><span class="sxs-lookup"><span data-stu-id="a5047-119">**ReportTemplate element values**</span></span>

|<span data-ttu-id="a5047-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a5047-120">**Value**</span></span>|<span data-ttu-id="a5047-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5047-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5047-122">Сводка</span><span class="sxs-lookup"><span data-stu-id="a5047-122">Summary</span></span>  <br/> |<span data-ttu-id="a5047-123">Указывает, что отчет будет отображаться всех получателей сообщения, а также состояние доставки сообщения для каждого получателя.</span><span class="sxs-lookup"><span data-stu-id="a5047-123">Specifies that the report will display all the recipients of the message and the delivery status of the message to each recipient.</span></span>  <br/> |
|<span data-ttu-id="a5047-124">RecipientPath</span><span class="sxs-lookup"><span data-stu-id="a5047-124">RecipientPath</span></span>  <br/> |<span data-ttu-id="a5047-125">Указывает, что для одного получателя, отчет будет отображаться с помощью журнала событий, возникших.</span><span class="sxs-lookup"><span data-stu-id="a5047-125">Specifies that for a single recipient, the report will display a full history of the events that occurred.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a5047-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="a5047-126">Remarks</span></span>

<span data-ttu-id="a5047-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a5047-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a5047-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a5047-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a5047-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a5047-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a5047-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a5047-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a5047-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a5047-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a5047-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a5047-132">Validation File</span></span>  <br/> |<span data-ttu-id="a5047-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a5047-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a5047-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a5047-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a5047-135">False</span><span class="sxs-lookup"><span data-stu-id="a5047-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a5047-136">См. также</span><span class="sxs-lookup"><span data-stu-id="a5047-136">See also</span></span>



- [<span data-ttu-id="a5047-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5047-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

