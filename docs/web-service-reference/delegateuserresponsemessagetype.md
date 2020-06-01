---
title: делегатеусерреспонсемессажетипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUserResponseMessageType
api_type:
- schema
ms.assetid: 3dc9552c-1e2d-40ac-a137-827883c2bb88
description: Элемент Делегатеусерреспонсемессажетипе содержит ответное сообщение для одного делегированного пользователя.
ms.openlocfilehash: d7addac2ef05d50e0043490ac20d299ece7d577b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457384"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="6d8ed-103">делегатеусерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="6d8ed-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="6d8ed-104">Элемент **делегатеусерреспонсемессажетипе** содержит ответное сообщение для одного делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="6d8ed-105">**делегатеусерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="6d8ed-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6d8ed-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6d8ed-106">Attributes and elements</span></span>

<span data-ttu-id="6d8ed-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d8ed-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6d8ed-108">Attributes</span></span>

<span data-ttu-id="6d8ed-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d8ed-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6d8ed-110">Child elements</span></span>

|<span data-ttu-id="6d8ed-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d8ed-111">**Element**</span></span>|<span data-ttu-id="6d8ed-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d8ed-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d8ed-113">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6d8ed-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6d8ed-114">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6d8ed-115">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6d8ed-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6d8ed-116">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6d8ed-117">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6d8ed-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6d8ed-118">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="6d8ed-119">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6d8ed-120">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="6d8ed-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6d8ed-121">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="6d8ed-122">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="6d8ed-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="6d8ed-123">Определяет один делегат, который возвращается в ответе управления представителями.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d8ed-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6d8ed-124">Parent elements</span></span>

|<span data-ttu-id="6d8ed-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d8ed-125">**Element**</span></span>|<span data-ttu-id="6d8ed-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d8ed-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d8ed-127">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="6d8ed-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="6d8ed-128">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6d8ed-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="6d8ed-129">Remarks</span></span>

<span data-ttu-id="6d8ed-130">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6d8ed-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6d8ed-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6d8ed-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d8ed-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6d8ed-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6d8ed-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6d8ed-133">Schema Name</span></span>  <br/> |<span data-ttu-id="6d8ed-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6d8ed-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6d8ed-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6d8ed-135">Validation File</span></span>  <br/> |<span data-ttu-id="6d8ed-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6d8ed-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6d8ed-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6d8ed-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d8ed-138">False</span><span class="sxs-lookup"><span data-stu-id="6d8ed-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d8ed-139">См. также</span><span class="sxs-lookup"><span data-stu-id="6d8ed-139">See also</span></span>

- [<span data-ttu-id="6d8ed-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6d8ed-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="6d8ed-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="6d8ed-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="6d8ed-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6d8ed-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="6d8ed-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="6d8ed-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="6d8ed-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6d8ed-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

