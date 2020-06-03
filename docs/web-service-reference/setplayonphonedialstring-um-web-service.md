---
title: SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: Элемент SetPlayOnPhoneDialString определяет запрос на установку строки набора номера по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена сообщениями) и запросов PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 40021e9dedafb5fafda91bf3612d8a6485dae8e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458630"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="b7391-103">SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="b7391-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="b7391-104">Элемент **SetPlayOnPhoneDialString** определяет запрос на установку строки набора номера по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md) и запросов [PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="b7391-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="b7391-105">SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="b7391-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="b7391-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="b7391-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7391-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b7391-107">Attributes and elements</span></span>

<span data-ttu-id="b7391-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b7391-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7391-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b7391-109">Attributes</span></span>

<span data-ttu-id="b7391-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b7391-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b7391-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b7391-111">Child elements</span></span>

|<span data-ttu-id="b7391-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b7391-112">**Element**</span></span>|<span data-ttu-id="b7391-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7391-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7391-114">dialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="b7391-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="b7391-115">Номер телефона, который необходимо задать в качестве строки набора по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="b7391-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7391-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b7391-116">Parent elements</span></span>

<span data-ttu-id="b7391-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b7391-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b7391-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b7391-118">Text value</span></span>

<span data-ttu-id="b7391-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b7391-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7391-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b7391-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7391-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b7391-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7391-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b7391-122">Schema Name</span></span>  <br/> |<span data-ttu-id="b7391-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="b7391-123">Messages</span></span>  <br/> |
|<span data-ttu-id="b7391-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b7391-124">Validation File</span></span>  <br/> |<span data-ttu-id="b7391-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b7391-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7391-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b7391-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7391-127">False</span><span class="sxs-lookup"><span data-stu-id="b7391-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7391-128">См. также</span><span class="sxs-lookup"><span data-stu-id="b7391-128">See also</span></span>



[<span data-ttu-id="b7391-129">Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="b7391-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

