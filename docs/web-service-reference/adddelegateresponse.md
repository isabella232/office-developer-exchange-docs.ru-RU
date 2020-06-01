---
title: аддделегатереспонсе
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
description: Элемент Аддделегатереспонсе содержит состояние и результат запроса операции AddDelegate.
ms.openlocfilehash: 1c38563ab38facf89fd5eab119542374949244c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466460"
---
# <a name="adddelegateresponse"></a><span data-ttu-id="76228-103">аддделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="76228-103">AddDelegateResponse</span></span>

<span data-ttu-id="76228-104">Элемент **аддделегатереспонсе** содержит состояние и результат запроса [операции AddDelegate](adddelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="76228-104">The **AddDelegateResponse** element contains the status and result of an [AddDelegate operation](adddelegate-operation.md) request.</span></span> 
  
```xml
<AddDelegateResponse>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</AddDelegateResponse>
```

 <span data-ttu-id="76228-105">**аддделегатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="76228-105">**AddDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76228-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="76228-106">Attributes and elements</span></span>

<span data-ttu-id="76228-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="76228-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76228-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="76228-108">Attributes</span></span>

<span data-ttu-id="76228-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="76228-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76228-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="76228-110">Child elements</span></span>

|<span data-ttu-id="76228-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="76228-111">**Element**</span></span>|<span data-ttu-id="76228-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="76228-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76228-113">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="76228-113">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="76228-114">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="76228-114">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="76228-115">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="76228-115">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="76228-116">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="76228-116">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="76228-117">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="76228-117">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="76228-118">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="76228-118">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="76228-119">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="76228-119">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="76228-120">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="76228-120">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="76228-121">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="76228-121">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="76228-122">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="76228-122">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="76228-123">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="76228-123">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76228-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="76228-124">Parent elements</span></span>

<span data-ttu-id="76228-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="76228-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="76228-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="76228-126">Remarks</span></span>

<span data-ttu-id="76228-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="76228-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76228-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="76228-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76228-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="76228-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76228-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="76228-130">Schema Name</span></span>  <br/> |<span data-ttu-id="76228-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="76228-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76228-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="76228-132">Validation File</span></span>  <br/> |<span data-ttu-id="76228-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="76228-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76228-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="76228-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="76228-135">False</span><span class="sxs-lookup"><span data-stu-id="76228-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76228-136">См. также</span><span class="sxs-lookup"><span data-stu-id="76228-136">See also</span></span>

- [<span data-ttu-id="76228-137">Операция AddDelegate</span><span class="sxs-lookup"><span data-stu-id="76228-137">AddDelegate operation</span></span>](adddelegate-operation.md)
- [<span data-ttu-id="76228-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="76228-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="76228-139">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="76228-139">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

