---
title: AddDelegateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegateResponse
api_type:
- schema
ms.assetid: d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429
description: Элемент AddDelegateResponse содержит состояние и результат запроса AddDelegate операции.
ms.openlocfilehash: a1d56e9994b3a7916fe0fbe40be1e6d8ff473730
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761334"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="45b4f-103">AddDelegateResponse</span><span class="sxs-lookup"><span data-stu-id="45b4f-103">AddDelegateResponse</span></span>

<span data-ttu-id="45b4f-104">Элемент **AddDelegateResponse** содержит состояние и результат [операции AddDelegate](adddelegate-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="45b4f-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="45b4f-105">**AddDelegateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="45b4f-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45b4f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="45b4f-106">Attributes and elements</span></span>

<span data-ttu-id="45b4f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="45b4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45b4f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="45b4f-108">Attributes</span></span>

<span data-ttu-id="45b4f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="45b4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45b4f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="45b4f-110">Child elements</span></span>

|<span data-ttu-id="45b4f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="45b4f-111">**Element**</span></span>|<span data-ttu-id="45b4f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="45b4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45b4f-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="45b4f-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="45b4f-114">Содержит сообщения ответа на запрос управления delegate веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="45b4f-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="45b4f-115">MessageText</span><span class="sxs-lookup"><span data-stu-id="45b4f-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="45b4f-116">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="45b4f-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="45b4f-117">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="45b4f-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="45b4f-118">Содержит код ошибки, которая идентифицирует ошибку, с которым возникла запроса.</span><span class="sxs-lookup"><span data-stu-id="45b4f-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="45b4f-119">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="45b4f-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="45b4f-120">В настоящее время неиспользуемых и зарезервирован для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="45b4f-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="45b4f-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="45b4f-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="45b4f-122">MessageXml</span><span class="sxs-lookup"><span data-stu-id="45b4f-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="45b4f-123">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="45b4f-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45b4f-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="45b4f-124">Parent elements</span></span>

<span data-ttu-id="45b4f-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="45b4f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45b4f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="45b4f-126">Remarks</span></span>

<span data-ttu-id="45b4f-127">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="45b4f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45b4f-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="45b4f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45b4f-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="45b4f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45b4f-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="45b4f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="45b4f-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="45b4f-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="45b4f-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="45b4f-132">Validation File</span></span>  <br/> |<span data-ttu-id="45b4f-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45b4f-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45b4f-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="45b4f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="45b4f-135">False</span><span class="sxs-lookup"><span data-stu-id="45b4f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45b4f-136">См. также</span><span class="sxs-lookup"><span data-stu-id="45b4f-136">See also</span></span>

- [<span data-ttu-id="45b4f-137">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="45b4f-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="45b4f-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="45b4f-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="45b4f-139">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="45b4f-139">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)
