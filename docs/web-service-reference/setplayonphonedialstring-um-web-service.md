---
title: SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Элемент SetPlayOnPhoneDialString определяет запрос на присвоение строке звонка по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ) и запросы PlayOnPhoneGreeting операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835450"
---
# <a name="setplayonphonedialstring-um-web-service"></a><span data-ttu-id="2ae61-103">SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="2ae61-103">SetPlayOnPhoneDialString (UM web service)</span></span>

<span data-ttu-id="2ae61-104">Элемент **SetPlayOnPhoneDialString** определяет запрос для установки строке звонка по умолчанию для запросов [PlayOnPhone операция (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) , а [операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="2ae61-104">The **SetPlayOnPhoneDialString** element defines a request to set the default dial string for [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md) requests.</span></span> 
  
[<span data-ttu-id="2ae61-105">SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="2ae61-105">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 <span data-ttu-id="2ae61-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="2ae61-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ae61-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2ae61-107">Attributes and elements</span></span>

<span data-ttu-id="2ae61-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2ae61-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ae61-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2ae61-109">Attributes</span></span>

<span data-ttu-id="2ae61-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ae61-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ae61-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2ae61-111">Child elements</span></span>

|<span data-ttu-id="2ae61-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ae61-112">**Element**</span></span>|<span data-ttu-id="2ae61-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ae61-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ae61-114">dialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="2ae61-114">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="2ae61-115">Номер телефона, чтобы установить в качестве строке звонка по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2ae61-115">The telephone number to set as the default dial string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2ae61-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2ae61-116">Parent elements</span></span>

<span data-ttu-id="2ae61-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ae61-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2ae61-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2ae61-118">Text value</span></span>

<span data-ttu-id="2ae61-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="2ae61-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ae61-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2ae61-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ae61-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2ae61-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2ae61-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2ae61-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2ae61-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="2ae61-123">Messages</span></span>  <br/> |
|<span data-ttu-id="2ae61-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2ae61-124">Validation File</span></span>  <br/> |<span data-ttu-id="2ae61-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2ae61-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2ae61-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2ae61-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ae61-127">False</span><span class="sxs-lookup"><span data-stu-id="2ae61-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ae61-128">См. также</span><span class="sxs-lookup"><span data-stu-id="2ae61-128">See also</span></span>



[<span data-ttu-id="2ae61-129">Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="2ae61-129">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)

