---
title: base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- base64FolderId
api_type:
- schema
ms.assetid: 662f8f2f-49a7-4c7a-9065-98a02a49cfcd
description: Элемент base64FolderId содержит идентификатор папки, чтобы указать в качестве папки электронной почты по умолчанию, из которого единой системы обмена сообщениями считывает этих сообщений по телефону в запросе SetTelephoneAccessFolderEmail операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 7d710542418a717c6fcad243a22682e5840ebbd2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761546"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="54004-103">base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="54004-104">Элемент **base64FolderId** содержит идентификатор папки, чтобы указать в качестве папки электронной почты по умолчанию, из которого единой системы обмена сообщениями считывает этих сообщений по телефону в запрос [SetTelephoneAccessFolderEmail операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="54004-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="54004-105">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="54004-106">base64FolderId (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="54004-107">**string**</span><span class="sxs-lookup"><span data-stu-id="54004-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54004-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54004-108">Attributes and elements</span></span>

<span data-ttu-id="54004-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="54004-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54004-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54004-110">Attributes</span></span>

<span data-ttu-id="54004-111">Нет</span><span class="sxs-lookup"><span data-stu-id="54004-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54004-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54004-112">Child elements</span></span>

<span data-ttu-id="54004-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="54004-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54004-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54004-114">Parent elements</span></span>

|<span data-ttu-id="54004-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54004-115">**Element**</span></span>|<span data-ttu-id="54004-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54004-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54004-117">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="54004-118">Определяет запрос, чтобы задать папку телефонного доступа электронной почты.</span><span class="sxs-lookup"><span data-stu-id="54004-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54004-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="54004-119">Text value</span></span>

<span data-ttu-id="54004-120">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="54004-120">A text value is required.</span></span> <span data-ttu-id="54004-121">Текстовое значение представляет идентификатор MAPI папки.</span><span class="sxs-lookup"><span data-stu-id="54004-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="54004-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="54004-122">Remarks</span></span>

<span data-ttu-id="54004-123">Чтобы задать папку телефонного доступа электронной почты, с помощью [операции SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="54004-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54004-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54004-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54004-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54004-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="54004-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54004-126">Schema Name</span></span>  <br/> |<span data-ttu-id="54004-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="54004-127">Messages</span></span>  <br/> |
|<span data-ttu-id="54004-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54004-128">Validation File</span></span>  <br/> |<span data-ttu-id="54004-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="54004-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="54004-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54004-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="54004-131">False</span><span class="sxs-lookup"><span data-stu-id="54004-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54004-132">См. также</span><span class="sxs-lookup"><span data-stu-id="54004-132">See also</span></span>



[<span data-ttu-id="54004-133">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="54004-134">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="54004-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="54004-135">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="54004-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="54004-136">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="54004-136">FindItem operation</span></span>](finditem-operation.md)

