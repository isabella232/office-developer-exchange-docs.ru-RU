---
title: форвардтореЦипиентс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ForwardToRecipients
api_type:
- schema
ms.assetid: dd58fd72-591d-4891-b226-465bcf12c19b
description: Элемент ForwardToRecipients указывает адреса электронной почты, к которым сообщения, для перенаправления.
ms.openlocfilehash: f2538f62bb9d837ef64bdc742b01d26d3d7d77f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762643"
---
# <a name="forwardtorecipients"></a><span data-ttu-id="fb3e9-103">форвардтореЦипиентс</span><span class="sxs-lookup"><span data-stu-id="fb3e9-103">ForwardToRecipients</span></span>

<span data-ttu-id="fb3e9-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Элемент **ForwardToRecipients** указывает адреса электронной почты, к которым сообщения, для перенаправления.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-104">The **ForwardToRecipients** element indicates the e-mail addresses to which messages are to be forwarded.</span></span> 
  
```XML
<ForwardToRecipients>
   <Address/>
</ForwardToRecipients>
```

 <span data-ttu-id="fb3e9-105">**аррайофемаиладдрессестипе**</span><span class="sxs-lookup"><span data-stu-id="fb3e9-105">**ArrayOfEmailAddressesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb3e9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fb3e9-106">Attributes and elements</span></span>

<span data-ttu-id="fb3e9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb3e9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fb3e9-108">Attributes</span></span>

<span data-ttu-id="fb3e9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb3e9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fb3e9-110">Child elements</span></span>

|<span data-ttu-id="fb3e9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb3e9-111">**Element**</span></span>|<span data-ttu-id="fb3e9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3e9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3e9-113">Адрес (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="fb3e9-113">Address (EmailAddressType)</span></span>](address-emailaddresstype.md) <br/> |<span data-ttu-id="fb3e9-114">Представляет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-114">Represents a fully resolved e-mail address.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fb3e9-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fb3e9-115">Parent elements</span></span>

|<span data-ttu-id="fb3e9-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fb3e9-116">**Element**</span></span>|<span data-ttu-id="fb3e9-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fb3e9-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb3e9-118">Действия</span><span class="sxs-lookup"><span data-stu-id="fb3e9-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="fb3e9-119">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb3e9-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fb3e9-120">Text value</span></span>

<span data-ttu-id="fb3e9-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fb3e9-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="fb3e9-122">Remarks</span></span>

<span data-ttu-id="fb3e9-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb3e9-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb3e9-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fb3e9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb3e9-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fb3e9-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fb3e9-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fb3e9-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fb3e9-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fb3e9-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fb3e9-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fb3e9-128">Validation File</span></span>  <br/> |<span data-ttu-id="fb3e9-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="fb3e9-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fb3e9-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fb3e9-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb3e9-131">True</span><span class="sxs-lookup"><span data-stu-id="fb3e9-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb3e9-132">См. также</span><span class="sxs-lookup"><span data-stu-id="fb3e9-132">See also</span></span>



- [<span data-ttu-id="fb3e9-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fb3e9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

