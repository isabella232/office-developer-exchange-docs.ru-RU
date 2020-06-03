---
title: испермиссионконтроллед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPermissionControlled
api_type:
- schema
ms.assetid: a2fd0340-f31f-4389-a1cd-7e93b40bb3c6
description: Элемент Испермиссионконтроллед указывает, должны ли входящие сообщения управляться разрешениями (RMS protected), чтобы применялось условие или исключение.
ms.openlocfilehash: 5fba06c1c56512f4a362f773f119ea346a4c0d2b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460388"
---
# <a name="ispermissioncontrolled"></a><span data-ttu-id="0e136-103">испермиссионконтроллед</span><span class="sxs-lookup"><span data-stu-id="0e136-103">IsPermissionControlled</span></span>

<span data-ttu-id="0e136-104">Элемент **испермиссионконтроллед** указывает, должны ли входящие сообщения управляться разрешениями (RMS protected), чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0e136-104">The **IsPermissionControlled** element indicates whether incoming messages must be permission controlled (RMS protected) in order for the condition or exception to apply.</span></span> 
  
```XML
<IsPermissionControlled>true | false</IsPermissionControlled>
```

 <span data-ttu-id="0e136-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="0e136-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e136-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0e136-106">Attributes and elements</span></span>

<span data-ttu-id="0e136-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0e136-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e136-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0e136-108">Attributes</span></span>

<span data-ttu-id="0e136-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0e136-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e136-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0e136-110">Child elements</span></span>

<span data-ttu-id="0e136-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0e136-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e136-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0e136-112">Parent elements</span></span>

|<span data-ttu-id="0e136-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0e136-113">**Element**</span></span>|<span data-ttu-id="0e136-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0e136-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e136-115">Условия</span><span class="sxs-lookup"><span data-stu-id="0e136-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="0e136-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="0e136-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="0e136-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="0e136-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="0e136-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="0e136-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e136-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0e136-119">Text value</span></span>

<span data-ttu-id="0e136-120">Текстовое значение **true** указывает, что сообщение должно быть защищено службой управления правами для применения условия или исключения.</span><span class="sxs-lookup"><span data-stu-id="0e136-120">A text value of **true** indicates that the message must be RMS protected in order for the condition or exception to apply.</span></span> <span data-ttu-id="0e136-121">Значение **false** указывает, что сообщение не должно быть защищено службой управления правами, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="0e136-121">A value of **false** indicates that the message must not be RMS protected in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="0e136-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="0e136-122">Remarks</span></span>

<span data-ttu-id="0e136-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0e136-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e136-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0e136-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e136-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0e136-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0e136-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0e136-126">Schema Name</span></span>  <br/> |<span data-ttu-id="0e136-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0e136-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0e136-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0e136-128">Validation File</span></span>  <br/> |<span data-ttu-id="0e136-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0e136-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0e136-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0e136-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e136-131">True</span><span class="sxs-lookup"><span data-stu-id="0e136-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e136-132">См. также</span><span class="sxs-lookup"><span data-stu-id="0e136-132">See also</span></span>



- [<span data-ttu-id="0e136-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0e136-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

