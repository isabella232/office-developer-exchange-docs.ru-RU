---
title: IsEncrypted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEncrypted
api_type:
- schema
ms.assetid: 68a30e92-c2b1-4af5-bb16-ba38afb80c43
description: Элемент "с шифрованием" указывает, должны ли входящие сообщения шифроваться с помощью параметра S/MIME, чтобы применить условие или исключение.
ms.openlocfilehash: 582a1f197d4ee6b60af91b1a178d79163b50052c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834003"
---
# <a name="isencrypted"></a><span data-ttu-id="39071-103">IsEncrypted</span><span class="sxs-lookup"><span data-stu-id="39071-103">IsEncrypted</span></span>

<span data-ttu-id="39071-104">Элемент "с **шифрованием** " указывает, должны ли входящие сообщения шифроваться с помощью параметра S/MIME, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="39071-104">The **IsEncrypted** element indicates whether incoming messages must be S/MIME encrypted in order for the condition or exception to apply.</span></span> 
  
```XML
<IsEncrypted>true | false</IsEncrypted>
```

 <span data-ttu-id="39071-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="39071-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39071-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="39071-106">Attributes and elements</span></span>

<span data-ttu-id="39071-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="39071-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39071-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="39071-108">Attributes</span></span>

<span data-ttu-id="39071-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="39071-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39071-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="39071-110">Child elements</span></span>

<span data-ttu-id="39071-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="39071-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="39071-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="39071-112">Parent elements</span></span>

|<span data-ttu-id="39071-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39071-113">**Element**</span></span>|<span data-ttu-id="39071-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39071-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39071-115">Условия</span><span class="sxs-lookup"><span data-stu-id="39071-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="39071-116">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="39071-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="39071-117">Исключения</span><span class="sxs-lookup"><span data-stu-id="39071-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="39071-118">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="39071-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="39071-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="39071-119">Text value</span></span>

<span data-ttu-id="39071-120">Текстовое значение **true** указывает, что сообщение должно быть зашифровано с помощью параметра S/MIME, чтобы применить условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="39071-120">A text value of **true** indicates that the message must be S/MIME encrypted in order for the condition or exception to apply.</span></span> <span data-ttu-id="39071-121">Значение **false** указывает, что сообщение не обязательно должно быть S/MIME, чтобы применялось условие или исключение.</span><span class="sxs-lookup"><span data-stu-id="39071-121">A value of **false** indicates that the message does not have to be S/MIME in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="39071-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="39071-122">Remarks</span></span>

<span data-ttu-id="39071-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="39071-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39071-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="39071-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39071-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="39071-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39071-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="39071-126">Schema Name</span></span>  <br/> |<span data-ttu-id="39071-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="39071-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39071-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="39071-128">Validation File</span></span>  <br/> |<span data-ttu-id="39071-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="39071-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39071-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="39071-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="39071-131">True</span><span class="sxs-lookup"><span data-stu-id="39071-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39071-132">См. также</span><span class="sxs-lookup"><span data-stu-id="39071-132">See also</span></span>



- [<span data-ttu-id="39071-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39071-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

