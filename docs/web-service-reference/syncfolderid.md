---
title: SyncFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: Элемент SyncFolderId представляет папку, содержащую элементы для синхронизации.
ms.openlocfilehash: 45a4a62c7d269861555089019db259eacab26ef0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840123"
---
# <a name="syncfolderid"></a><span data-ttu-id="6cc52-103">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="6cc52-103">SyncFolderId</span></span>

<span data-ttu-id="6cc52-104">Элемент **SyncFolderId** представляет папку, содержащую элементы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="6cc52-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

 <span data-ttu-id="6cc52-105">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="6cc52-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cc52-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6cc52-106">Attributes and elements</span></span>

<span data-ttu-id="6cc52-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6cc52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cc52-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6cc52-108">Attributes</span></span>

<span data-ttu-id="6cc52-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cc52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cc52-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6cc52-110">Child elements</span></span>

|<span data-ttu-id="6cc52-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6cc52-111">**Element**</span></span>|<span data-ttu-id="6cc52-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cc52-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cc52-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="6cc52-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="6cc52-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="6cc52-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="6cc52-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="6cc52-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="6cc52-116">Идентифицирует MicrosoftExchange Server 2007 папок, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="6cc52-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cc52-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6cc52-117">Parent elements</span></span>

|<span data-ttu-id="6cc52-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6cc52-118">**Element**</span></span>|<span data-ttu-id="6cc52-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cc52-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cc52-120">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="6cc52-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="6cc52-121">Определяет запрос для синхронизации иерархии папок в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cc52-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6cc52-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6cc52-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="6cc52-123">Определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="6cc52-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6cc52-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="6cc52-124">Remarks</span></span>

<span data-ttu-id="6cc52-125">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6cc52-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cc52-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6cc52-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cc52-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6cc52-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cc52-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6cc52-128">Schema name</span></span>  <br/> |<span data-ttu-id="6cc52-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6cc52-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cc52-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6cc52-130">Validation file</span></span>  <br/> |<span data-ttu-id="6cc52-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cc52-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cc52-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6cc52-132">Can be empty</span></span>  <br/> |<span data-ttu-id="6cc52-133">False</span><span class="sxs-lookup"><span data-stu-id="6cc52-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cc52-134">См. также</span><span class="sxs-lookup"><span data-stu-id="6cc52-134">See also</span></span>



[<span data-ttu-id="6cc52-135">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6cc52-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6cc52-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cc52-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

