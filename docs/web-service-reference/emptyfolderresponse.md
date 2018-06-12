---
title: EmptyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: Элемент EmptyFolderResponse определяет ответа на запрос операции EmptyFolder.
ms.openlocfilehash: ab753351a1eb7deba83823875989816ba75b9809
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762325"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="c9192-103">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c9192-103">EmptyFolderResponse</span></span>

<span data-ttu-id="c9192-104">Элемент **EmptyFolderResponse** определяет ответ на запрос [EmptyFolder операции](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c9192-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="c9192-105">**EmptyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="c9192-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c9192-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c9192-106">Attributes and elements</span></span>

<span data-ttu-id="c9192-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c9192-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c9192-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c9192-108">Attributes</span></span>

<span data-ttu-id="c9192-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9192-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c9192-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c9192-110">Child elements</span></span>

|<span data-ttu-id="c9192-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c9192-111">**Element**</span></span>|<span data-ttu-id="c9192-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c9192-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c9192-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c9192-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c9192-114">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9192-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c9192-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c9192-115">Parent elements</span></span>

<span data-ttu-id="c9192-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="c9192-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c9192-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="c9192-117">Remarks</span></span>

<span data-ttu-id="c9192-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c9192-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c9192-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c9192-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c9192-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c9192-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c9192-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c9192-121">Schema name</span></span>  <br/> |<span data-ttu-id="c9192-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c9192-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c9192-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c9192-123">Validation file</span></span>  <br/> |<span data-ttu-id="c9192-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c9192-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c9192-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c9192-125">Can be empty</span></span>  <br/> |<span data-ttu-id="c9192-126">False</span><span class="sxs-lookup"><span data-stu-id="c9192-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c9192-127">См. также</span><span class="sxs-lookup"><span data-stu-id="c9192-127">See also</span></span>



[<span data-ttu-id="c9192-128">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="c9192-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="c9192-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="c9192-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="c9192-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c9192-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

