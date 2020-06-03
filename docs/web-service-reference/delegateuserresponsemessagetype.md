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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457384"
---
# <a name="delegateuserresponsemessagetype"></a><span data-ttu-id="bcdee-103">делегатеусерреспонсемессажетипе</span><span class="sxs-lookup"><span data-stu-id="bcdee-103">DelegateUserResponseMessageType</span></span>

<span data-ttu-id="bcdee-104">Элемент **делегатеусерреспонсемессажетипе** содержит ответное сообщение для одного делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="bcdee-104">The **DelegateUserResponseMessageType** element contains the response message for a single delegate user.</span></span> 
  
```xml
<DelegateUserResponseMessageType>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DelegateUser/>
</DelegateUserResponseMessageType>
```

<span data-ttu-id="bcdee-105">**делегатеусерреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="bcdee-105">**DelegateUserResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bcdee-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bcdee-106">Attributes and elements</span></span>

<span data-ttu-id="bcdee-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bcdee-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bcdee-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bcdee-108">Attributes</span></span>

<span data-ttu-id="bcdee-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bcdee-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bcdee-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bcdee-110">Child elements</span></span>

|<span data-ttu-id="bcdee-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bcdee-111">**Element**</span></span>|<span data-ttu-id="bcdee-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bcdee-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcdee-113">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bcdee-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bcdee-114">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="bcdee-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bcdee-115">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bcdee-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bcdee-116">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="bcdee-116">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bcdee-117">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bcdee-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bcdee-118">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="bcdee-118">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="bcdee-119">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="bcdee-119">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bcdee-120">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="bcdee-120">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bcdee-121">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="bcdee-121">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bcdee-122">делегатеусер</span><span class="sxs-lookup"><span data-stu-id="bcdee-122">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="bcdee-123">Определяет один делегат, который возвращается в ответе управления представителями.</span><span class="sxs-lookup"><span data-stu-id="bcdee-123">Identifies a single delegate that is returned in a delegate management response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bcdee-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bcdee-124">Parent elements</span></span>

|<span data-ttu-id="bcdee-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bcdee-125">**Element**</span></span>|<span data-ttu-id="bcdee-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bcdee-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bcdee-127">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="bcdee-127">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="bcdee-128">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="bcdee-128">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bcdee-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="bcdee-129">Remarks</span></span>

<span data-ttu-id="bcdee-130">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bcdee-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bcdee-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bcdee-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bcdee-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bcdee-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bcdee-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bcdee-133">Schema Name</span></span>  <br/> |<span data-ttu-id="bcdee-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bcdee-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bcdee-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bcdee-135">Validation File</span></span>  <br/> |<span data-ttu-id="bcdee-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bcdee-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bcdee-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bcdee-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="bcdee-138">False</span><span class="sxs-lookup"><span data-stu-id="bcdee-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bcdee-139">См. также</span><span class="sxs-lookup"><span data-stu-id="bcdee-139">See also</span></span>

- [<span data-ttu-id="bcdee-140">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="bcdee-140">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="bcdee-141">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="bcdee-141">GetDelegate operation</span></span>](getdelegate-operation.md) 
- [<span data-ttu-id="bcdee-142">Операция UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="bcdee-142">UpdateDelegate operation</span></span>](updatedelegate-operation.md)  
- [<span data-ttu-id="bcdee-143">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="bcdee-143">RemoveDelegate operation</span></span>](removedelegate-operation.md)
- [<span data-ttu-id="bcdee-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bcdee-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

