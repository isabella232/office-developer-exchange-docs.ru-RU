---
title: аутлукрулеблобексистс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: Элемент Аутлукрулеблобексистс указывает, существует ли большой двоичный объект правила Microsoft Outlook в почтовом ящике пользователя.
ms.openlocfilehash: 6a5c2a2ec0246d38b22279b86772972ea81922c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529030"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="73cfe-103">аутлукрулеблобексистс</span><span class="sxs-lookup"><span data-stu-id="73cfe-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="73cfe-104">Элемент **аутлукрулеблобексистс** указывает, существует ли большой двоичный объект правила Microsoft Outlook в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="73cfe-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="73cfe-105">жетинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="73cfe-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="73cfe-106">аутлукрулеблобексистс</span><span class="sxs-lookup"><span data-stu-id="73cfe-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="73cfe-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="73cfe-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73cfe-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="73cfe-108">Attributes and elements</span></span>

<span data-ttu-id="73cfe-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="73cfe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73cfe-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="73cfe-110">Attributes</span></span>

<span data-ttu-id="73cfe-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73cfe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73cfe-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="73cfe-112">Child elements</span></span>

<span data-ttu-id="73cfe-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="73cfe-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="73cfe-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="73cfe-114">Parent elements</span></span>

|<span data-ttu-id="73cfe-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="73cfe-115">**Element**</span></span>|<span data-ttu-id="73cfe-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="73cfe-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73cfe-117">жетинбоксрулесреспонсе</span><span class="sxs-lookup"><span data-stu-id="73cfe-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="73cfe-118">Представляет ответ на запрос [операции GetInboxRules](getinboxrules-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="73cfe-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="73cfe-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="73cfe-119">Text value</span></span>

<span data-ttu-id="73cfe-120">Текстовое значение **true** указывает, что существует большой двоичный объект правила Outlook.</span><span class="sxs-lookup"><span data-stu-id="73cfe-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="73cfe-121">Текстовое значение **false** указывает, что большой двоичный объект правила Outlook не существует.</span><span class="sxs-lookup"><span data-stu-id="73cfe-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="73cfe-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="73cfe-122">Remarks</span></span>

<span data-ttu-id="73cfe-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="73cfe-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73cfe-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="73cfe-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73cfe-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="73cfe-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="73cfe-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="73cfe-126">Schema Name</span></span>  <br/> |<span data-ttu-id="73cfe-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="73cfe-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="73cfe-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="73cfe-128">Validation File</span></span>  <br/> |<span data-ttu-id="73cfe-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="73cfe-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73cfe-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="73cfe-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="73cfe-131">True</span><span class="sxs-lookup"><span data-stu-id="73cfe-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="73cfe-132">См. также</span><span class="sxs-lookup"><span data-stu-id="73cfe-132">See also</span></span>



- [<span data-ttu-id="73cfe-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="73cfe-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

