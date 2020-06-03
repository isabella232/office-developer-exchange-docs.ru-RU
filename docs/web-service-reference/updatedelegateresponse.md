---
title: упдатеделегатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateDelegateResponse
api_type:
- schema
ms.assetid: cd336add-fbcc-4f61-9867-d4c08a60e142
description: Элемент Упдатеделегатереспонсе содержит состояние и результат запроса операции UpdateDelegate.
ms.openlocfilehash: 9f11d87ac07dd51a5231d4546fac92e7ca95ad4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465053"
---
# <a name="updatedelegateresponse"></a><span data-ttu-id="b0b61-103">упдатеделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="b0b61-103">UpdateDelegateResponse</span></span>

<span data-ttu-id="b0b61-104">Элемент **упдатеделегатереспонсе** содержит состояние и результат запроса [операции UpdateDelegate](updatedelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="b0b61-104">The **UpdateDelegateResponse** element contains the status and result of an [UpdateDelegate operation](updatedelegate-operation.md) request.</span></span> 
  
```xml
<UpdateDelegateResponseMessage>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateDelegateResponseMessage>
```

 <span data-ttu-id="b0b61-105">**упдатеделегатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="b0b61-105">**UpdateDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0b61-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0b61-106">Attributes and elements</span></span>

<span data-ttu-id="b0b61-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b0b61-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0b61-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0b61-108">Attributes</span></span>

<span data-ttu-id="b0b61-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b0b61-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0b61-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0b61-110">Child elements</span></span>

|<span data-ttu-id="b0b61-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0b61-111">**Element**</span></span>|<span data-ttu-id="b0b61-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0b61-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0b61-113">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="b0b61-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="b0b61-114">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b0b61-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="b0b61-115">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b0b61-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b0b61-116">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="b0b61-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b0b61-117">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b0b61-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b0b61-118">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="b0b61-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b0b61-119">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b0b61-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b0b61-120">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="b0b61-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b0b61-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="b0b61-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b0b61-122">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="b0b61-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b0b61-123">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b0b61-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b0b61-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0b61-124">Parent elements</span></span>

<span data-ttu-id="b0b61-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="b0b61-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0b61-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="b0b61-126">Remarks</span></span>

<span data-ttu-id="b0b61-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b0b61-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b0b61-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0b61-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0b61-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0b61-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b0b61-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0b61-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b0b61-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b0b61-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b0b61-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0b61-132">Validation File</span></span>  <br/> |<span data-ttu-id="b0b61-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b0b61-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b0b61-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0b61-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0b61-135">False</span><span class="sxs-lookup"><span data-stu-id="b0b61-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0b61-136">См. также</span><span class="sxs-lookup"><span data-stu-id="b0b61-136">See also</span></span>



[<span data-ttu-id="b0b61-137">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="b0b61-137">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="b0b61-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b0b61-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

