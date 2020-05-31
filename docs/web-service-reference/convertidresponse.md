---
title: конвертидреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertIdResponse
api_type:
- schema
ms.assetid: ac1f044f-04a4-42ef-b762-cac5cd37894d
description: Элемент Конвертидреспонсе содержит ответ на запрос ConvertId. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 80299afebcebf15546b0fdbe14f0b08960527a47
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761828"
---
# <a name="convertidresponse"></a><span data-ttu-id="f1589-104">конвертидреспонсе</span><span class="sxs-lookup"><span data-stu-id="f1589-104">ConvertIdResponse</span></span>

<span data-ttu-id="f1589-105">Элемент **конвертидреспонсе** содержит ответ на запрос ConvertId.</span><span class="sxs-lookup"><span data-stu-id="f1589-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="f1589-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f1589-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="f1589-107">**конвертидреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="f1589-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1589-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1589-108">Attributes and elements</span></span>

<span data-ttu-id="f1589-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f1589-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1589-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1589-110">Attributes</span></span>

<span data-ttu-id="f1589-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1589-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1589-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1589-112">Child elements</span></span>

|<span data-ttu-id="f1589-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1589-113">**Element**</span></span>|<span data-ttu-id="f1589-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1589-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1589-115">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f1589-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f1589-116">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1589-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1589-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1589-117">Parent elements</span></span>

<span data-ttu-id="f1589-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1589-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f1589-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f1589-119">Remarks</span></span>

<span data-ttu-id="f1589-120">Сообщения ответа, содержащиеся в элементе [респонсемессажес](responsemessages.md) , будут экземплярами конвертидреспонсемессажетипе.</span><span class="sxs-lookup"><span data-stu-id="f1589-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="f1589-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f1589-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1589-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1589-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1589-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1589-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f1589-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1589-124">Schema Name</span></span>  <br/> |<span data-ttu-id="f1589-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f1589-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f1589-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1589-126">Validation File</span></span>  <br/> |<span data-ttu-id="f1589-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f1589-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f1589-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1589-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1589-129">False</span><span class="sxs-lookup"><span data-stu-id="f1589-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1589-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f1589-130">See also</span></span>



[<span data-ttu-id="f1589-131">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="f1589-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="f1589-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1589-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f1589-133">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="f1589-133">Converting Identifiers</span></span>](http://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

