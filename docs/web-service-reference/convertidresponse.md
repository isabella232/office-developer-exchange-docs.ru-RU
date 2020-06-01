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
ms.openlocfilehash: 690f0f2109dfc36dd8f359b7cef1e65beb47fc6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452526"
---
# <a name="convertidresponse"></a><span data-ttu-id="76b23-104">конвертидреспонсе</span><span class="sxs-lookup"><span data-stu-id="76b23-104">ConvertIdResponse</span></span>

<span data-ttu-id="76b23-105">Элемент **конвертидреспонсе** содержит ответ на запрос ConvertId.</span><span class="sxs-lookup"><span data-stu-id="76b23-105">The **ConvertIdResponse** element contains a response to a ConvertId request.</span></span> <span data-ttu-id="76b23-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="76b23-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ConvertIdResponse>
   <ResponseMessages/>
</ConvertIdResponse>
```

 <span data-ttu-id="76b23-107">**конвертидреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="76b23-107">**ConvertIdResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76b23-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="76b23-108">Attributes and elements</span></span>

<span data-ttu-id="76b23-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="76b23-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76b23-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="76b23-110">Attributes</span></span>

<span data-ttu-id="76b23-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76b23-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76b23-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="76b23-112">Child elements</span></span>

|<span data-ttu-id="76b23-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76b23-113">**Element**</span></span>|<span data-ttu-id="76b23-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76b23-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76b23-115">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="76b23-115">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="76b23-116">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="76b23-116">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76b23-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="76b23-117">Parent elements</span></span>

<span data-ttu-id="76b23-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="76b23-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="76b23-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="76b23-119">Remarks</span></span>

<span data-ttu-id="76b23-120">Сообщения ответа, содержащиеся в элементе [респонсемессажес](responsemessages.md) , будут экземплярами конвертидреспонсемессажетипе.</span><span class="sxs-lookup"><span data-stu-id="76b23-120">The response messages that are contained within the [ResponseMessages](responsemessages.md) element will be instances of ConvertIdResponseMessageType.</span></span> 
  
<span data-ttu-id="76b23-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="76b23-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76b23-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="76b23-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76b23-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="76b23-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76b23-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="76b23-124">Schema Name</span></span>  <br/> |<span data-ttu-id="76b23-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="76b23-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76b23-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="76b23-126">Validation File</span></span>  <br/> |<span data-ttu-id="76b23-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="76b23-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76b23-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="76b23-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="76b23-129">False</span><span class="sxs-lookup"><span data-stu-id="76b23-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76b23-130">См. также</span><span class="sxs-lookup"><span data-stu-id="76b23-130">See also</span></span>



[<span data-ttu-id="76b23-131">Операция ConvertId</span><span class="sxs-lookup"><span data-stu-id="76b23-131">ConvertId operation</span></span>](convertid-operation.md)


- [<span data-ttu-id="76b23-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="76b23-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="76b23-133">Преобразование идентификаторов</span><span class="sxs-lookup"><span data-stu-id="76b23-133">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)

