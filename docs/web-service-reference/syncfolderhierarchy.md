---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: Элемент SyncFolderHierarchy определяет запрос для синхронизации иерархии папок на клиенте.
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840122"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="a4735-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a4735-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="a4735-104">Элемент **SyncFolderHierarchy** определяет запрос для синхронизации иерархии папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="a4735-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="a4735-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="a4735-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4735-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a4735-106">Attributes and elements</span></span>

<span data-ttu-id="a4735-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a4735-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4735-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a4735-108">Attributes</span></span>

<span data-ttu-id="a4735-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4735-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4735-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a4735-110">Child elements</span></span>

|<span data-ttu-id="a4735-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a4735-111">**Element**</span></span>|<span data-ttu-id="a4735-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a4735-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4735-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="a4735-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="a4735-114">Задает свойства папки для включения в [SyncFolderHierarchy](syncfolderhierarchy.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="a4735-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="a4735-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="a4735-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="a4735-116">Представляет папку, содержащую элементы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a4735-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="a4735-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a4735-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a4735-118">Состояние</span><span class="sxs-lookup"><span data-stu-id="a4735-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a4735-119">Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="a4735-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="a4735-120">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a4735-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4735-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a4735-121">Parent elements</span></span>

<span data-ttu-id="a4735-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4735-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a4735-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="a4735-123">Remarks</span></span>

<span data-ttu-id="a4735-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a4735-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4735-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a4735-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4735-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a4735-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4735-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a4735-127">Schema name</span></span>  <br/> |<span data-ttu-id="a4735-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a4735-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4735-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a4735-129">Validation file</span></span>  <br/> |<span data-ttu-id="a4735-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a4735-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4735-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a4735-131">Can be empty</span></span>  <br/> |<span data-ttu-id="a4735-132">False</span><span class="sxs-lookup"><span data-stu-id="a4735-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4735-133">См. также</span><span class="sxs-lookup"><span data-stu-id="a4735-133">See also</span></span>



[<span data-ttu-id="a4735-134">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="a4735-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="a4735-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a4735-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

