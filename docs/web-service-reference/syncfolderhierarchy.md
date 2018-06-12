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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840122"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="c4620-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c4620-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="c4620-104">Элемент **SyncFolderHierarchy** определяет запрос для синхронизации иерархии папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="c4620-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="c4620-105">**SyncFolderHierarchyType**</span><span class="sxs-lookup"><span data-stu-id="c4620-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4620-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c4620-106">Attributes and elements</span></span>

<span data-ttu-id="c4620-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c4620-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4620-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c4620-108">Attributes</span></span>

<span data-ttu-id="c4620-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4620-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4620-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c4620-110">Child elements</span></span>

|<span data-ttu-id="c4620-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c4620-111">**Element**</span></span>|<span data-ttu-id="c4620-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4620-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4620-113">FolderShape</span><span class="sxs-lookup"><span data-stu-id="c4620-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="c4620-114">Задает свойства папки для включения в [SyncFolderHierarchy](syncfolderhierarchy.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="c4620-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="c4620-115">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="c4620-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="c4620-116">Представляет папку, содержащую элементы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c4620-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="c4620-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="c4620-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="c4620-118">Состояние</span><span class="sxs-lookup"><span data-stu-id="c4620-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c4620-119">Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="c4620-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="c4620-120">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="c4620-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4620-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c4620-121">Parent elements</span></span>

<span data-ttu-id="c4620-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4620-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4620-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="c4620-123">Remarks</span></span>

<span data-ttu-id="c4620-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c4620-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4620-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c4620-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4620-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c4620-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4620-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c4620-127">Schema name</span></span>  <br/> |<span data-ttu-id="c4620-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c4620-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c4620-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c4620-129">Validation file</span></span>  <br/> |<span data-ttu-id="c4620-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c4620-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4620-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c4620-131">Can be empty</span></span>  <br/> |<span data-ttu-id="c4620-132">False</span><span class="sxs-lookup"><span data-stu-id="c4620-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4620-133">См. также</span><span class="sxs-lookup"><span data-stu-id="c4620-133">See also</span></span>



[<span data-ttu-id="c4620-134">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c4620-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="c4620-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c4620-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

