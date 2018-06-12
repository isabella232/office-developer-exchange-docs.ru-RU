---
title: PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 206a2ad1-a01d-4e71-99a1-90c2530423da
description: Элемент PlayOnPhone определяет запрос для воспроизведения на телефоне элемента.
ms.openlocfilehash: 7e5c1e25512a59d1ac3295b476fcc2b6b0f5a2b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834825"
---
# <a name="playonphone-um-web-service"></a><span data-ttu-id="7f0d0-103">PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="7f0d0-103">PlayOnPhone (UM web service)</span></span>

<span data-ttu-id="7f0d0-104">Элемент **PlayOnPhone** определяет запрос для воспроизведения на телефоне элемента.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-104">The **PlayOnPhone** element defines a request to play an item on a telephone.</span></span> 
  
[<span data-ttu-id="7f0d0-105">PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="7f0d0-105">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
```xml
<PlayOnPhone>
  <entryId>   </entryId>
  <DialString>   </DialString>
</PlayOnPhone>
```

 <span data-ttu-id="7f0d0-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="7f0d0-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f0d0-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7f0d0-107">Attributes and elements</span></span>

<span data-ttu-id="7f0d0-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f0d0-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7f0d0-109">Attributes</span></span>

<span data-ttu-id="7f0d0-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7f0d0-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7f0d0-111">Child elements</span></span>

|<span data-ttu-id="7f0d0-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7f0d0-112">**Element**</span></span>|<span data-ttu-id="7f0d0-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7f0d0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f0d0-114">Идентификатор записи (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="7f0d0-114">entryId (UM web service)</span></span>](entryid-um-web-service.md) <br/> |<span data-ttu-id="7f0d0-115">Содержит значение, представляющее идентификатор элемента для воспроизведения на телефоне в запрос [PlayOnPhone операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="7f0d0-115">Contains the value that represents the identifier of the item to play on the telephone in a [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) request.</span></span>  <br/> |
|[<span data-ttu-id="7f0d0-116">dialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="7f0d0-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md) <br/> |<span data-ttu-id="7f0d0-117">Содержит значение, номер телефона для набора номера.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-117">Contains the value for the telephone number to dial.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f0d0-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7f0d0-118">Parent elements</span></span>

<span data-ttu-id="7f0d0-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="7f0d0-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7f0d0-120">Text value</span></span>

<span data-ttu-id="7f0d0-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="7f0d0-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f0d0-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7f0d0-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f0d0-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7f0d0-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f0d0-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7f0d0-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7f0d0-125">Сообщения</span><span class="sxs-lookup"><span data-stu-id="7f0d0-125">Messages</span></span>  <br/> |
|<span data-ttu-id="7f0d0-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7f0d0-126">Validation File</span></span>  <br/> |<span data-ttu-id="7f0d0-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f0d0-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f0d0-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7f0d0-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f0d0-129">False</span><span class="sxs-lookup"><span data-stu-id="7f0d0-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f0d0-130">См. также</span><span class="sxs-lookup"><span data-stu-id="7f0d0-130">See also</span></span>



[<span data-ttu-id="7f0d0-131">Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="7f0d0-131">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)

