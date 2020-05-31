---
title: SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetTelephoneAccessFolderEmail
api_type:
- schema
ms.assetid: 90759da7-6dba-499e-b8c8-e44a016b3198
description: Элемент SetTelephoneAccessFolderEmail определяет запрос на установку папки электронной почты по умолчанию, из которой единая система обмена сообщениями будет читать сообщения по телефону.
ms.openlocfilehash: e19f151e364411717d5129cbef8c5cc097689f89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835461"
---
# <a name="settelephoneaccessfolderemail-um-web-service"></a><span data-ttu-id="eace0-103">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="eace0-103">SetTelephoneAccessFolderEmail (UM web service)</span></span>

<span data-ttu-id="eace0-104">Элемент **SetTelephoneAccessFolderEmail** определяет запрос на установку папки электронной почты по умолчанию, из которой единая система обмена сообщениями будет читать сообщения по телефону.</span><span class="sxs-lookup"><span data-stu-id="eace0-104">The **SetTelephoneAccessFolderEmail** element defines a request to set the default e-mail folder from which Unified Messaging will read messages over the telephone.</span></span> 
  
[<span data-ttu-id="eace0-105">SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="eace0-105">SetTelephoneAccessFolderEmail (UM web service)</span></span>](settelephoneaccessfolderemail-um-web-service.md)
  
```xml
<SetTelephoneAccessFolderEmail>
  <base64FolderId>   </base64FolderId>
</SetTelephoneAccessFolderEmail>
```

 <span data-ttu-id="eace0-106">**complexType**</span><span class="sxs-lookup"><span data-stu-id="eace0-106">**complexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eace0-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eace0-107">Attributes and elements</span></span>

<span data-ttu-id="eace0-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="eace0-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eace0-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eace0-109">Attributes</span></span>

<span data-ttu-id="eace0-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="eace0-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eace0-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eace0-111">Child elements</span></span>

|<span data-ttu-id="eace0-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eace0-112">**Element**</span></span>|<span data-ttu-id="eace0-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eace0-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eace0-114">base64FolderId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="eace0-114">base64FolderId (UM web service)</span></span>](base64folderid-um-web-service.md) <br/> |<span data-ttu-id="eace0-115">Идентификатор папки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="eace0-115">The identifier of the e-mail folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eace0-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eace0-116">Parent elements</span></span>

<span data-ttu-id="eace0-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="eace0-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="eace0-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="eace0-118">Text value</span></span>

<span data-ttu-id="eace0-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="eace0-119">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eace0-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eace0-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eace0-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eace0-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eace0-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eace0-122">Schema Name</span></span>  <br/> |<span data-ttu-id="eace0-123">Сообщения</span><span class="sxs-lookup"><span data-stu-id="eace0-123">Messages</span></span>  <br/> |
|<span data-ttu-id="eace0-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eace0-124">Validation File</span></span>  <br/> |<span data-ttu-id="eace0-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="eace0-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eace0-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eace0-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="eace0-127">False</span><span class="sxs-lookup"><span data-stu-id="eace0-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eace0-128">См. также</span><span class="sxs-lookup"><span data-stu-id="eace0-128">See also</span></span>



[<span data-ttu-id="eace0-129">Операция SetTelephoneAccessFolderEmail (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="eace0-129">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)

