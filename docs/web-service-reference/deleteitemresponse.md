---
title: DeleteItemResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponse
api_type:
- schema
ms.assetid: 86463d66-fe47-4a19-a81b-e24841e816ab
description: Элемент DeleteItemResponse определяет ответа на один запрос DeleteItem.
ms.openlocfilehash: 8a35033c744fbcb0829d2c79a8d79557f77137bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762045"
---
# <a name="deleteitemresponse"></a><span data-ttu-id="03691-103">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="03691-103">DeleteItemResponse</span></span>

<span data-ttu-id="03691-104">Элемент **DeleteItemResponse** определяет ответа на один запрос DeleteItem.</span><span class="sxs-lookup"><span data-stu-id="03691-104">The **DeleteItemResponse** element defines a response to a single DeleteItem request.</span></span> 
  
```xml
<DeleteItemResponse>
   <ResponseMessages/>
</DeleteItemResponse>
```

 <span data-ttu-id="03691-105">**DeleteItemResponseType**</span><span class="sxs-lookup"><span data-stu-id="03691-105">**DeleteItemResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03691-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03691-106">Attributes and elements</span></span>

<span data-ttu-id="03691-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="03691-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03691-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03691-108">Attributes</span></span>

<span data-ttu-id="03691-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="03691-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03691-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03691-110">Child elements</span></span>

|<span data-ttu-id="03691-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03691-111">**Element**</span></span>|<span data-ttu-id="03691-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03691-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03691-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="03691-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="03691-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="03691-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03691-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03691-115">Parent elements</span></span>

<span data-ttu-id="03691-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="03691-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="03691-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="03691-117">Remarks</span></span>

<span data-ttu-id="03691-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="03691-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03691-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="03691-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03691-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="03691-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03691-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="03691-121">Schema Name</span></span>  <br/> |<span data-ttu-id="03691-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="03691-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03691-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="03691-123">Validation File</span></span>  <br/> |<span data-ttu-id="03691-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="03691-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03691-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="03691-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="03691-126">False</span><span class="sxs-lookup"><span data-stu-id="03691-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03691-127">См. также</span><span class="sxs-lookup"><span data-stu-id="03691-127">See also</span></span>

- [<span data-ttu-id="03691-128">Операция DeleteItem</span><span class="sxs-lookup"><span data-stu-id="03691-128">DeleteItem operation</span></span>](deleteitem-operation.md)  
- [<span data-ttu-id="03691-129">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="03691-129">DeleteItem</span></span>](deleteitem.md)
- [<span data-ttu-id="03691-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="03691-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
