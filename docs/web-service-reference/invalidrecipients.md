---
title: инвалидреЦипиентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipients
api_type:
- schema
ms.assetid: e4e7b50e-2fa9-4649-94a6-6002f341ecc4
description: Элемент InvalidRecipients представляет получателей запрос на общий доступ к папке, которые являются недопустимыми.
ms.openlocfilehash: 99e0817f0ff873c4732b03cc7d68aa8e0070813c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465564"
---
# <a name="invalidrecipients"></a><span data-ttu-id="a0e9e-103">инвалидреЦипиентс</span><span class="sxs-lookup"><span data-stu-id="a0e9e-103">InvalidRecipients</span></span>

<span data-ttu-id="a0e9e-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **InvalidRecipients** представляет получателей запрос на общий доступ к папке, которые являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-104">The **InvalidRecipients** element represents the recipients of a folder sharing request that are invalid.</span></span> 
  
```XML
<InvalidRecipients>
   <InvalidRecipient/>
</InvalidRecipients>
```

 <span data-ttu-id="a0e9e-105">**аррайофинвалидреЦипиентстипе**</span><span class="sxs-lookup"><span data-stu-id="a0e9e-105">**ArrayOfInvalidRecipientsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0e9e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a0e9e-106">Attributes and elements</span></span>

<span data-ttu-id="a0e9e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0e9e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a0e9e-108">Attributes</span></span>

<span data-ttu-id="a0e9e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0e9e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a0e9e-110">Child elements</span></span>

|<span data-ttu-id="a0e9e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0e9e-111">**Element**</span></span>|<span data-ttu-id="a0e9e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0e9e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0e9e-113">инвалидреЦипиент</span><span class="sxs-lookup"><span data-stu-id="a0e9e-113">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="a0e9e-114">Содержит SMTP-адрес недопустимого получателя и сведения о почему получатель является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-114">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a0e9e-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a0e9e-115">Parent elements</span></span>

|<span data-ttu-id="a0e9e-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0e9e-116">**Element**</span></span>|<span data-ttu-id="a0e9e-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0e9e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0e9e-118">жетшарингметадатареспонсе</span><span class="sxs-lookup"><span data-stu-id="a0e9e-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="a0e9e-119">Определяет ответ на запрос [Операция GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a0e9e-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="a0e9e-120">жетшарингметадатареспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a0e9e-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="a0e9e-121">Содержит состояние и результат одного [Операция GetSharingMetadata](getsharingmetadata-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a0e9e-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="a0e9e-122">Remarks</span></span>

<span data-ttu-id="a0e9e-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a0e9e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0e9e-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a0e9e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0e9e-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a0e9e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a0e9e-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a0e9e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="a0e9e-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a0e9e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a0e9e-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a0e9e-128">Validation File</span></span>  <br/> |<span data-ttu-id="a0e9e-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a0e9e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a0e9e-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a0e9e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="a0e9e-131">False</span><span class="sxs-lookup"><span data-stu-id="a0e9e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a0e9e-132">См. также</span><span class="sxs-lookup"><span data-stu-id="a0e9e-132">See also</span></span>



[<span data-ttu-id="a0e9e-133">Операция GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="a0e9e-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="a0e9e-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a0e9e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

