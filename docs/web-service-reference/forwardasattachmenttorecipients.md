---
title: ForwardAsAttachmentToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardAsAttachmentToRecipients
api_type:
- schema
ms.assetid: 8649ea14-672f-43c9-b10a-a2b02efd5867
description: Элемент ForwardAsAttachmentToRecipients указывает адреса электронной почты, к которым сообщения, пересылаемые в виде вложений.
ms.openlocfilehash: 04d4f9c6228e6d0ab34a6eff5d5751f461a57e19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762641"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="b10f4-103">ForwardAsAttachmentToRecipients</span><span class="sxs-lookup"><span data-stu-id="b10f4-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="b10f4-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **ForwardAsAttachmentToRecipients** указывает адреса электронной почты, к которым сообщения, пересылаемые в виде вложений.</span><span class="sxs-lookup"><span data-stu-id="b10f4-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="b10f4-105">**ArrayOfEmailAddressesType**</span><span class="sxs-lookup"><span data-stu-id="b10f4-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b10f4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b10f4-106">Attributes and elements</span></span>

<span data-ttu-id="b10f4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b10f4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b10f4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b10f4-108">Attributes</span></span>

<span data-ttu-id="b10f4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b10f4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b10f4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b10f4-110">Child elements</span></span>

|<span data-ttu-id="b10f4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b10f4-111">**Element**</span></span>|<span data-ttu-id="b10f4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b10f4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b10f4-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b10f4-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="b10f4-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="b10f4-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b10f4-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b10f4-115">Parent elements</span></span>

|<span data-ttu-id="b10f4-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b10f4-116">**Element**</span></span>|<span data-ttu-id="b10f4-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b10f4-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b10f4-118">Действия</span><span class="sxs-lookup"><span data-stu-id="b10f4-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="b10f4-119">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="b10f4-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b10f4-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b10f4-120">Text value</span></span>

<span data-ttu-id="b10f4-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="b10f4-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b10f4-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="b10f4-122">Remarks</span></span>

<span data-ttu-id="b10f4-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b10f4-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b10f4-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b10f4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b10f4-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b10f4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b10f4-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b10f4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="b10f4-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b10f4-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b10f4-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b10f4-128">Validation File</span></span>  <br/> |<span data-ttu-id="b10f4-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b10f4-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b10f4-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b10f4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="b10f4-131">True</span><span class="sxs-lookup"><span data-stu-id="b10f4-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b10f4-132">См. также</span><span class="sxs-lookup"><span data-stu-id="b10f4-132">See also</span></span>



- [<span data-ttu-id="b10f4-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b10f4-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

