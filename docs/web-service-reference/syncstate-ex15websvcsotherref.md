---
title: синкстате
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: Элемент Синкстате содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса. Используется для определения состояния синхронизации.
ms.openlocfilehash: 8e2d9a633cdad0a124b87e4e794399c06d3b5445
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458966"
---
# <a name="syncstate"></a><span data-ttu-id="b27ef-104">синкстате</span><span class="sxs-lookup"><span data-stu-id="b27ef-104">SyncState</span></span>

<span data-ttu-id="b27ef-105">Элемент **синкстате** содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="b27ef-105">The **SyncState** element contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="b27ef-106">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="b27ef-106">This is used to identify the synchronization state.</span></span> 
  
```xml
<SyncState/>
```

 <span data-ttu-id="b27ef-107">**String**</span><span class="sxs-lookup"><span data-stu-id="b27ef-107">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b27ef-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b27ef-108">Attributes and elements</span></span>

<span data-ttu-id="b27ef-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b27ef-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b27ef-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b27ef-110">Attributes</span></span>

<span data-ttu-id="b27ef-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b27ef-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b27ef-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b27ef-112">Child elements</span></span>

<span data-ttu-id="b27ef-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b27ef-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b27ef-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b27ef-114">Parent elements</span></span>

|<span data-ttu-id="b27ef-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b27ef-115">**Element**</span></span>|<span data-ttu-id="b27ef-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b27ef-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b27ef-117">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b27ef-117">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="b27ef-118">Определяет запрос на синхронизацию иерархии папок в клиенте.</span><span class="sxs-lookup"><span data-stu-id="b27ef-118">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> |
|[<span data-ttu-id="b27ef-119">синкфолдерхиерарчиреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b27ef-119">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md) <br/> |<span data-ttu-id="b27ef-120">Содержит состояние и результат запроса SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="b27ef-120">Contains the status and result of a SyncFolderHierarchy request.</span></span>  <br/> |
|[<span data-ttu-id="b27ef-121">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b27ef-121">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="b27ef-122">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="b27ef-122">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
|[<span data-ttu-id="b27ef-123">синкфолдеритемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="b27ef-123">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md) <br/> |<span data-ttu-id="b27ef-124">Содержит состояние и результат запроса SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="b27ef-124">Contains the status and result of a SyncFolderItems request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b27ef-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b27ef-125">Text value</span></span>

<span data-ttu-id="b27ef-126">При использовании этого элемента необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="b27ef-126">A text value is required when this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b27ef-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="b27ef-127">Remarks</span></span>

<span data-ttu-id="b27ef-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b27ef-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b27ef-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b27ef-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b27ef-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b27ef-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b27ef-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b27ef-131">Schema name</span></span>  <br/> |<span data-ttu-id="b27ef-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b27ef-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b27ef-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b27ef-133">Validation file</span></span>  <br/> |<span data-ttu-id="b27ef-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b27ef-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b27ef-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b27ef-135">Can be empty</span></span>  <br/> |<span data-ttu-id="b27ef-136">False</span><span class="sxs-lookup"><span data-stu-id="b27ef-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b27ef-137">См. также</span><span class="sxs-lookup"><span data-stu-id="b27ef-137">See also</span></span>



[<span data-ttu-id="b27ef-138">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="b27ef-138">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
  
[<span data-ttu-id="b27ef-139">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="b27ef-139">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="b27ef-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b27ef-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

