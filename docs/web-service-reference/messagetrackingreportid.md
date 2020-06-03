---
title: мессажетраккингрепортид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReportId
api_type:
- schema
ms.assetid: 9c604ca3-10fe-4760-b7fd-8b52f1a0c712
description: Элемент Мессажетраккингрепортид представляет сообщение с помощью идентификатора сообщения, Организации, в которой было найдено сообщение, сервера, на котором было отправлено сообщение, а также внутреннего идентификатора, уникально идентифицирующего сообщение.
ms.openlocfilehash: d6e92593d55608e260634602c2aab694804d716d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460598"
---
# <a name="messagetrackingreportid"></a><span data-ttu-id="33143-103">мессажетраккингрепортид</span><span class="sxs-lookup"><span data-stu-id="33143-103">MessageTrackingReportId</span></span>

<span data-ttu-id="33143-104">Элемент **мессажетраккингрепортид** представляет сообщение с помощью идентификатора сообщения, Организации, в которой было найдено сообщение, сервера, на котором было отправлено сообщение, а также внутреннего идентификатора, уникально идентифицирующего сообщение.</span><span class="sxs-lookup"><span data-stu-id="33143-104">The **MessageTrackingReportId** element represents the message by its message ID, the organization where the message was found, the server on which the message was submitted, and an internal ID that uniquely identifies the message.</span></span> 
  
```XML
<MessageTrackingReportId/>
```

 <span data-ttu-id="33143-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="33143-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33143-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33143-106">Attributes and elements</span></span>

<span data-ttu-id="33143-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33143-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33143-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33143-108">Attributes</span></span>

<span data-ttu-id="33143-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33143-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33143-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33143-110">Child elements</span></span>

<span data-ttu-id="33143-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="33143-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33143-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33143-112">Parent elements</span></span>

|<span data-ttu-id="33143-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33143-113">**Element**</span></span>|<span data-ttu-id="33143-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33143-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33143-115">GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="33143-115">GetMessageTrackingReport</span></span>](getmessagetrackingreport.md) <br/> |<span data-ttu-id="33143-116">Содержит запрос для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) , чтобы получить полный отчет об отслеживании сообщений для указанного идентификатора.</span><span class="sxs-lookup"><span data-stu-id="33143-116">Contains the request for the [GetMessageTrackingReport operation](getmessagetrackingreport-operation.md) to retrieve the full message tracking report for the specified ID.</span></span>  <br/> |
|[<span data-ttu-id="33143-117">мессажетраккингсеарчресулт</span><span class="sxs-lookup"><span data-stu-id="33143-117">MessageTrackingSearchResult</span></span>](messagetrackingsearchresult.md) <br/> |<span data-ttu-id="33143-118">Содержит один результат одного сообщения для элемента [финдмессажетраккингрепортреспонсе](findmessagetrackingreportresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="33143-118">Contains a single message result for a [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33143-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33143-119">Text value</span></span>

<span data-ttu-id="33143-120">При использовании этого элемента необходимо указать текстовое значение, представляющее строку.</span><span class="sxs-lookup"><span data-stu-id="33143-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33143-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="33143-121">Remarks</span></span>

<span data-ttu-id="33143-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="33143-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33143-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33143-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33143-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33143-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33143-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33143-125">Schema Name</span></span>  <br/> |<span data-ttu-id="33143-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33143-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="33143-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33143-127">Validation File</span></span>  <br/> |<span data-ttu-id="33143-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33143-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33143-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33143-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="33143-130">False</span><span class="sxs-lookup"><span data-stu-id="33143-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33143-131">См. также</span><span class="sxs-lookup"><span data-stu-id="33143-131">See also</span></span>



[<span data-ttu-id="33143-132">Операция GetMessageTrackingReport</span><span class="sxs-lookup"><span data-stu-id="33143-132">GetMessageTrackingReport operation</span></span>](getmessagetrackingreport-operation.md)


- [<span data-ttu-id="33143-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="33143-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

