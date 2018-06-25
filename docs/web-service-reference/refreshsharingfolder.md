---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: Элемент RefreshSharingFolder определяет запрос на обновление указанного локальную папку. Это базовый элемент для операции RefreshSharingFolder.
ms.openlocfilehash: b09e311d0ba38b0cdcc9fe0864ed3e2b0151b0fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835043"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="37b6b-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="37b6b-104">RefreshSharingFolder</span></span>

<span data-ttu-id="37b6b-105">Элемент **RefreshSharingFolder** определяет запрос на обновление указанного локальную папку.</span><span class="sxs-lookup"><span data-stu-id="37b6b-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="37b6b-106">Это базовый элемент для [операции RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="37b6b-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="37b6b-107">**RefreshSharingFolderType**</span><span class="sxs-lookup"><span data-stu-id="37b6b-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="37b6b-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="37b6b-108">Attributes and elements</span></span>

<span data-ttu-id="37b6b-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="37b6b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="37b6b-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="37b6b-110">Attributes</span></span>

<span data-ttu-id="37b6b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="37b6b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="37b6b-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="37b6b-112">Child elements</span></span>

|<span data-ttu-id="37b6b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="37b6b-113">**Element**</span></span>|<span data-ttu-id="37b6b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="37b6b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="37b6b-115">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="37b6b-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="37b6b-116">Представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="37b6b-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="37b6b-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="37b6b-117">Parent elements</span></span>

<span data-ttu-id="37b6b-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="37b6b-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="37b6b-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="37b6b-119">Remarks</span></span>

<span data-ttu-id="37b6b-120">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="37b6b-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="37b6b-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="37b6b-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="37b6b-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="37b6b-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="37b6b-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="37b6b-123">Schema Name</span></span>  <br/> |<span data-ttu-id="37b6b-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="37b6b-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="37b6b-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="37b6b-125">Validation File</span></span>  <br/> |<span data-ttu-id="37b6b-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="37b6b-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="37b6b-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="37b6b-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="37b6b-128">False</span><span class="sxs-lookup"><span data-stu-id="37b6b-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="37b6b-129">См. также</span><span class="sxs-lookup"><span data-stu-id="37b6b-129">See also</span></span>



- [<span data-ttu-id="37b6b-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37b6b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

