---
title: SharingFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingFolderId
api_type:
- schema
ms.assetid: 5ad37ceb-2922-4420-9051-c29d0d57c420
description: Элемент SharingFolderId представляет идентификатор локальной папки в отношении общего доступа.
ms.openlocfilehash: e0eb1fbd7155040508daf253f5eb4b1352d7426d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835485"
---
# <a name="sharingfolderid"></a><span data-ttu-id="0679a-103">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="0679a-103">SharingFolderId</span></span>

<span data-ttu-id="0679a-104">Элемент **SharingFolderId** представляет идентификатор локальной папки в отношении общего доступа.</span><span class="sxs-lookup"><span data-stu-id="0679a-104">The **SharingFolderId** element represents the identifier of the local folder in a sharing relationship.</span></span> 
  
```xml
<SharingFolderId Id="" ChangeKey="" />
```

 <span data-ttu-id="0679a-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0679a-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0679a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0679a-106">Attributes and elements</span></span>

<span data-ttu-id="0679a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0679a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0679a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0679a-108">Attributes</span></span>

|<span data-ttu-id="0679a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0679a-109">**Attribute**</span></span>|<span data-ttu-id="0679a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0679a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0679a-111">Id</span><span class="sxs-lookup"><span data-stu-id="0679a-111">Id</span></span>  <br/> |<span data-ttu-id="0679a-112">Содержит строку, которая определяет папке в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="0679a-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="0679a-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="0679a-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="0679a-114">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="0679a-114">ChangeKey</span></span>  <br/> |<span data-ttu-id="0679a-115">Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии.</span><span class="sxs-lookup"><span data-stu-id="0679a-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="0679a-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0679a-116">This attribute is optional.</span></span> <span data-ttu-id="0679a-117">Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.</span><span class="sxs-lookup"><span data-stu-id="0679a-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0679a-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0679a-118">Child elements</span></span>

<span data-ttu-id="0679a-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="0679a-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0679a-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0679a-120">Parent elements</span></span>

|<span data-ttu-id="0679a-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0679a-121">**Element**</span></span>|<span data-ttu-id="0679a-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0679a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0679a-123">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="0679a-123">RefreshSharingFolder</span></span>](refreshsharingfolder.md) <br/> |<span data-ttu-id="0679a-124">Определяет запрос на обновление указанного локальную папку.</span><span class="sxs-lookup"><span data-stu-id="0679a-124">Defines a request to refresh the specified local folder.</span></span>  <br/> |
|[<span data-ttu-id="0679a-125">GetSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0679a-125">GetSharingFolderResponse</span></span>](getsharingfolderresponse.md) <br/> |<span data-ttu-id="0679a-126">Определяет ответ на запрос [GetSharingFolder операции](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0679a-126">Defines a response to a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0679a-127">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0679a-127">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md) <br/> |<span data-ttu-id="0679a-128">Содержит состояние и результат одного запроса [GetSharingFolder операции](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="0679a-128">Contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0679a-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="0679a-129">Remarks</span></span>

<span data-ttu-id="0679a-130">Схема, описывающая этот элемент находится в IIS виртуального каталога веб-служб Exchange узлов компьютера, на котором выполняется Microsoft Exchange Server, на наличие установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0679a-130">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0679a-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0679a-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0679a-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0679a-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0679a-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0679a-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0679a-134">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0679a-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0679a-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0679a-135">Validation File</span></span>  <br/> |<span data-ttu-id="0679a-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0679a-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0679a-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0679a-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0679a-138">False</span><span class="sxs-lookup"><span data-stu-id="0679a-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0679a-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0679a-139">See also</span></span>



- [<span data-ttu-id="0679a-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0679a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

