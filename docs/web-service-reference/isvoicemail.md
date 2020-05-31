---
title: Голосовая почта
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsVoicemail
api_type:
- schema
ms.assetid: 96d81d6e-4b75-43ad-b151-2dd4fd57db94
description: Элемент IsVoicemail указывает, должен ли входящих сообщений сообщения голосовой почты в порядке для условие или исключение для применения.
ms.openlocfilehash: 513498301aa65eaf0cac5769c940eeedf5c9e629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834136"
---
# <a name="isvoicemail"></a><span data-ttu-id="be407-103">Голосовая почта</span><span class="sxs-lookup"><span data-stu-id="be407-103">IsVoicemail</span></span>

<span data-ttu-id="be407-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **IsVoicemail** указывает, должен ли входящих сообщений сообщения голосовой почты в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="be407-104">The **IsVoicemail** element indicates whether incoming messages must be voice mail messages in order for the condition or exception to apply.</span></span> 
  
```XML
<IsVoicemail>true | false</IsVoicemail>
```

 <span data-ttu-id="be407-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="be407-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be407-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="be407-106">Attributes and elements</span></span>

<span data-ttu-id="be407-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="be407-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be407-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="be407-108">Attributes</span></span>

<span data-ttu-id="be407-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="be407-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be407-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="be407-110">Child elements</span></span>

<span data-ttu-id="be407-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="be407-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be407-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="be407-112">Parent elements</span></span>

|<span data-ttu-id="be407-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="be407-113">**Element**</span></span>|<span data-ttu-id="be407-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="be407-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be407-115">Условия</span><span class="sxs-lookup"><span data-stu-id="be407-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="be407-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="be407-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="be407-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="be407-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="be407-118">Представляет исключения, которые представляют все доступные правила условия исключений для правила папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="be407-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be407-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="be407-119">Text value</span></span>

<span data-ttu-id="be407-p101">Текстовое значение **true** указывает, что сообщения должны быть сообщения голосовой почты в порядке для условие или исключение для применения. Значение **false** указывает, что сообщение не должна быть сообщения голосовой почты в порядке для условие или исключение для применения.</span><span class="sxs-lookup"><span data-stu-id="be407-p101">A text value of **true** indicates that the message must be a voice mail message in order for the condition or exception to apply. A value of **false** indicates that the message must not be a voice mail message in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="be407-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="be407-122">Remarks</span></span>

<span data-ttu-id="be407-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="be407-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be407-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="be407-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be407-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="be407-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be407-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="be407-126">Schema Name</span></span>  <br/> |<span data-ttu-id="be407-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="be407-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="be407-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="be407-128">Validation File</span></span>  <br/> |<span data-ttu-id="be407-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="be407-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be407-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="be407-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="be407-131">True</span><span class="sxs-lookup"><span data-stu-id="be407-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be407-132">См. также</span><span class="sxs-lookup"><span data-stu-id="be407-132">See also</span></span>



- [<span data-ttu-id="be407-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="be407-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

