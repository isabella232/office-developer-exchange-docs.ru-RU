---
title: ремоведелегатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegateResponse
api_type:
- schema
ms.assetid: eef56c53-d0a7-4342-9ce6-4dbb6b1a1369
description: Элемент Ремоведелегатереспонсе содержит состояние и результат запроса операции RemoveDelegate.
ms.openlocfilehash: 4c7a8b81528435b72576c116bc97f611544c24d6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468938"
---
# <a name="removedelegateresponse"></a><span data-ttu-id="7fb53-103">ремоведелегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="7fb53-103">RemoveDelegateResponse</span></span>

<span data-ttu-id="7fb53-104">Элемент **ремоведелегатереспонсе** содержит состояние и результат запроса [операции RemoveDelegate](removedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="7fb53-104">The **RemoveDelegateResponse** element contains the status and result of a [RemoveDelegate operation](removedelegate-operation.md) request.</span></span> 
  
```xml
<RemoveDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RemoveDelegateResponse>
```

 <span data-ttu-id="7fb53-105">**ремоведелегатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="7fb53-105">**RemoveDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7fb53-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7fb53-106">Attributes and elements</span></span>

<span data-ttu-id="7fb53-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7fb53-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7fb53-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7fb53-108">Attributes</span></span>

<span data-ttu-id="7fb53-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7fb53-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7fb53-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7fb53-110">Child elements</span></span>

|<span data-ttu-id="7fb53-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7fb53-111">**Element**</span></span>|<span data-ttu-id="7fb53-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7fb53-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7fb53-113">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="7fb53-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="7fb53-114">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7fb53-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="7fb53-115">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="7fb53-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7fb53-116">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="7fb53-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7fb53-117">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7fb53-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7fb53-118">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="7fb53-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7fb53-119">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="7fb53-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7fb53-120">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="7fb53-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7fb53-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="7fb53-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7fb53-122">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="7fb53-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7fb53-123">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7fb53-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7fb53-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7fb53-124">Parent elements</span></span>

<span data-ttu-id="7fb53-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="7fb53-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7fb53-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="7fb53-126">Remarks</span></span>

<span data-ttu-id="7fb53-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7fb53-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7fb53-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7fb53-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7fb53-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7fb53-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7fb53-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7fb53-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7fb53-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7fb53-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7fb53-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7fb53-132">Validation File</span></span>  <br/> |<span data-ttu-id="7fb53-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7fb53-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7fb53-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7fb53-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7fb53-135">False</span><span class="sxs-lookup"><span data-stu-id="7fb53-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7fb53-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7fb53-136">See also</span></span>



[<span data-ttu-id="7fb53-137">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="7fb53-137">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="7fb53-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7fb53-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

