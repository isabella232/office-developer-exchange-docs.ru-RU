---
title: base64FolderId (веб-служба единой системы обмена сообщениями)
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
description: Элемент base64FolderId содержит идентификатор папки, которую необходимо указать в качестве папки электронной почты по умолчанию, из которой единая система обмена сообщениями читает сообщения по телефону, в запросе веб-службы единой системы обмена сообщениями SetTelephoneAccessFolderEmail.
ms.openlocfilehash: ea31c7a0f93188e563bf95c4a3e6e91f0866746c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458049"
---
# <a name="base64folderid-um-web-service"></a><span data-ttu-id="1e38d-103">base64FolderId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-103">base64FolderId (UM web service)</span></span>

<span data-ttu-id="1e38d-104">Элемент **base64FolderId** содержит идентификатор папки, которую необходимо указать в качестве папки электронной почты по умолчанию, из которой единая система обмена сообщениями читает сообщения по телефону, в запросе [веб-службы единой системы обмена](settelephoneaccessfolderemail-operation-um-web-service.md) сообщениями SetTelephoneAccessFolderEmail.</span><span class="sxs-lookup"><span data-stu-id="1e38d-104">The **base64FolderId** element contains the identifier of the folder to specify as the default e-mail folder from which Unified Messaging reads messages over the telephone in a [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="1e38d-105">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="1e38d-106">base64FolderId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-106">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md)
  
```xml
<base64FolderId/>
```

 <span data-ttu-id="1e38d-107">**строка**</span><span class="sxs-lookup"><span data-stu-id="1e38d-107">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e38d-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1e38d-108">Attributes and elements</span></span>

<span data-ttu-id="1e38d-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1e38d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e38d-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1e38d-110">Attributes</span></span>

<span data-ttu-id="1e38d-111">Нет</span><span class="sxs-lookup"><span data-stu-id="1e38d-111">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e38d-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1e38d-112">Child elements</span></span>

<span data-ttu-id="1e38d-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1e38d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e38d-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1e38d-114">Parent elements</span></span>

|<span data-ttu-id="1e38d-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1e38d-115">**Element**</span></span>|<span data-ttu-id="1e38d-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1e38d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e38d-117">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-117">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="1e38d-118">Определяет запрос на установку папки электронной почты для телефонного доступа.</span><span class="sxs-lookup"><span data-stu-id="1e38d-118">Defines request to set the telephone access e-mail folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e38d-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1e38d-119">Text value</span></span>

<span data-ttu-id="1e38d-120">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="1e38d-120">A text value is required.</span></span> <span data-ttu-id="1e38d-121">Текстовое значение представляет идентификатор MAPI папки.</span><span class="sxs-lookup"><span data-stu-id="1e38d-121">The text value represents the MAPI ID of the folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e38d-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="1e38d-122">Remarks</span></span>

<span data-ttu-id="1e38d-123">Чтобы задать папку электронной почты для телефонного доступа, используйте [операцию SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)](settelephoneaccessfolderemail-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="1e38d-123">To set the telephone access e-mail folder, use the [SetTelephoneAccessFolderEmail operation (UM web service)](settelephoneaccessfolderemail-operation-um-web-service.md).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e38d-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1e38d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e38d-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1e38d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e38d-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1e38d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="1e38d-127">Сообщения</span><span class="sxs-lookup"><span data-stu-id="1e38d-127">Messages</span></span>  <br/> |
|<span data-ttu-id="1e38d-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1e38d-128">Validation File</span></span>  <br/> |<span data-ttu-id="1e38d-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1e38d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e38d-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1e38d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e38d-131">False</span><span class="sxs-lookup"><span data-stu-id="1e38d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e38d-132">См. также</span><span class="sxs-lookup"><span data-stu-id="1e38d-132">See also</span></span>



[<span data-ttu-id="1e38d-133">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-133">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
[<span data-ttu-id="1e38d-134">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1e38d-134">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
  
[<span data-ttu-id="1e38d-135">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="1e38d-135">FindFolder operation</span></span>](findfolder-operation.md)
  
[<span data-ttu-id="1e38d-136">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="1e38d-136">FindItem operation</span></span>](finditem-operation.md)

