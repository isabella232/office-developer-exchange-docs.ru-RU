---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: Элемент «подсказки» представляет получателей и типы советов по использованию почты, которые необходимо получить.
ms.openlocfilehash: 8ff71ed5d52f713e11188b07c8c93aeee7dfa44d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458637"
---
# <a name="getmailtips"></a><span data-ttu-id="4e331-103">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="4e331-103">GetMailTips</span></span>

<span data-ttu-id="4e331-104">Элемент « **подсказки** » представляет получателей и типы советов по использованию почты, которые необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="4e331-104">The **GetMailTips** element represents the recipients and types of mail tips to retrieve.</span></span> 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 <span data-ttu-id="4e331-105">**жетмаилтипстипе**</span><span class="sxs-lookup"><span data-stu-id="4e331-105">**GetMailTipsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e331-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4e331-106">Attributes and elements</span></span>

<span data-ttu-id="4e331-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4e331-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e331-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4e331-108">Attributes</span></span>

<span data-ttu-id="4e331-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e331-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e331-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4e331-110">Child elements</span></span>

|<span data-ttu-id="4e331-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e331-111">**Element**</span></span>|<span data-ttu-id="4e331-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e331-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e331-113">сендингас</span><span class="sxs-lookup"><span data-stu-id="4e331-113">SendingAs</span></span>](sendingas.md) <br/> |<span data-ttu-id="4e331-114">Содержит адрес электронной почты, который пользователь пытается отправить как.</span><span class="sxs-lookup"><span data-stu-id="4e331-114">Contains an e-mail address that a user is trying to send as.</span></span>  <br/> |
|[<span data-ttu-id="4e331-115">Получатели (АррайофреЦипиентстипе)</span><span class="sxs-lookup"><span data-stu-id="4e331-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="4e331-116">Содержит список получателей для проверки почтовых подсказок.</span><span class="sxs-lookup"><span data-stu-id="4e331-116">Contains a list of recipients to check for mail tips.</span></span>  <br/> |
|[<span data-ttu-id="4e331-117">маилтипсрекуестед</span><span class="sxs-lookup"><span data-stu-id="4e331-117">MailTipsRequested</span></span>](mailtipsrequested.md) <br/> |<span data-ttu-id="4e331-118">Содержит типы советов по использованию почты, запрошенных службой.</span><span class="sxs-lookup"><span data-stu-id="4e331-118">Contains the types of mail tips requested from the service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e331-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4e331-119">Parent elements</span></span>

<span data-ttu-id="4e331-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4e331-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4e331-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4e331-121">Text value</span></span>

<span data-ttu-id="4e331-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="4e331-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e331-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="4e331-123">Remarks</span></span>

<span data-ttu-id="4e331-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e331-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e331-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4e331-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e331-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4e331-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e331-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4e331-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4e331-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4e331-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4e331-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4e331-129">Validation File</span></span>  <br/> |<span data-ttu-id="4e331-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4e331-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e331-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4e331-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e331-132">False</span><span class="sxs-lookup"><span data-stu-id="4e331-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e331-133">См. также</span><span class="sxs-lookup"><span data-stu-id="4e331-133">See also</span></span>



- [<span data-ttu-id="4e331-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4e331-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

