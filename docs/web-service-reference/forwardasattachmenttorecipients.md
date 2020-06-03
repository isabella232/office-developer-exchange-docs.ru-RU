---
title: форвардасаттачменттореЦипиентс
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
ms.openlocfilehash: bf8c3563460eea811602074bf16f9253b4610832
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44453338"
---
# <a name="forwardasattachmenttorecipients"></a><span data-ttu-id="09b8a-103">форвардасаттачменттореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="09b8a-103">ForwardAsAttachmentToRecipients</span></span>

<span data-ttu-id="09b8a-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **ForwardAsAttachmentToRecipients** указывает адреса электронной почты, к которым сообщения, пересылаемые в виде вложений.</span><span class="sxs-lookup"><span data-stu-id="09b8a-104">The **ForwardAsAttachmentToRecipients** element indicates the e-mail addresses to which messages are to be forwarded as attachments.</span></span> 
  
```XML
<ForwardAsAttachmentToRecipients>
   <Address/>
</ForwardAsAttachmentToRecipients>
```

 <span data-ttu-id="09b8a-105">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="09b8a-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="09b8a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09b8a-106">Attributes and elements</span></span>

<span data-ttu-id="09b8a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="09b8a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09b8a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09b8a-108">Attributes</span></span>

<span data-ttu-id="09b8a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="09b8a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09b8a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09b8a-110">Child elements</span></span>

|<span data-ttu-id="09b8a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09b8a-111">**Element**</span></span>|<span data-ttu-id="09b8a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09b8a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09b8a-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="09b8a-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="09b8a-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="09b8a-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="09b8a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09b8a-115">Parent elements</span></span>

|<span data-ttu-id="09b8a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09b8a-116">**Element**</span></span>|<span data-ttu-id="09b8a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09b8a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09b8a-118">Действия</span><span class="sxs-lookup"><span data-stu-id="09b8a-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="09b8a-119">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="09b8a-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09b8a-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="09b8a-120">Text value</span></span>

<span data-ttu-id="09b8a-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="09b8a-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09b8a-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="09b8a-122">Remarks</span></span>

<span data-ttu-id="09b8a-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="09b8a-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="09b8a-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="09b8a-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="09b8a-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="09b8a-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="09b8a-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="09b8a-126">Schema Name</span></span>  <br/> |<span data-ttu-id="09b8a-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="09b8a-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="09b8a-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="09b8a-128">Validation File</span></span>  <br/> |<span data-ttu-id="09b8a-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="09b8a-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="09b8a-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="09b8a-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="09b8a-131">True</span><span class="sxs-lookup"><span data-stu-id="09b8a-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="09b8a-132">См. также</span><span class="sxs-lookup"><span data-stu-id="09b8a-132">See also</span></span>



- [<span data-ttu-id="09b8a-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="09b8a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

