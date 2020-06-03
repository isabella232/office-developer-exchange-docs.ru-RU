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
description: Элемент SyncFolderHierarchy определяет запрос на синхронизацию иерархии папок в клиенте.
ms.openlocfilehash: 68b607dbf603e955f74dfaccadd3ce6c4c9fb6ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466649"
---
# <a name="syncfolderhierarchy"></a><span data-ttu-id="bf42e-103">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="bf42e-103">SyncFolderHierarchy</span></span>

<span data-ttu-id="bf42e-104">Элемент **SyncFolderHierarchy** определяет запрос на синхронизацию иерархии папок в клиенте.</span><span class="sxs-lookup"><span data-stu-id="bf42e-104">The **SyncFolderHierarchy** element defines a request to synchronize a folder hierarchy on a client.</span></span> 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 <span data-ttu-id="bf42e-105">**синкфолдерхиерарчитипе**</span><span class="sxs-lookup"><span data-stu-id="bf42e-105">**SyncFolderHierarchyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bf42e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bf42e-106">Attributes and elements</span></span>

<span data-ttu-id="bf42e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bf42e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bf42e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bf42e-108">Attributes</span></span>

<span data-ttu-id="bf42e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bf42e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bf42e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bf42e-110">Child elements</span></span>

|<span data-ttu-id="bf42e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bf42e-111">**Element**</span></span>|<span data-ttu-id="bf42e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bf42e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bf42e-113">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="bf42e-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="bf42e-114">Определяет свойства папки, включаемые в ответ [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="bf42e-114">Identifies the folder properties to include in a [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span>  <br/> |
|[<span data-ttu-id="bf42e-115">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="bf42e-115">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="bf42e-116">Представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="bf42e-116">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="bf42e-117">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="bf42e-117">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="bf42e-118">синкстате</span><span class="sxs-lookup"><span data-stu-id="bf42e-118">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="bf42e-119">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="bf42e-119">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="bf42e-120">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bf42e-120">This is used to identify the synchronization state.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bf42e-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bf42e-121">Parent elements</span></span>

<span data-ttu-id="bf42e-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="bf42e-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bf42e-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="bf42e-123">Remarks</span></span>

<span data-ttu-id="bf42e-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bf42e-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bf42e-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bf42e-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bf42e-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bf42e-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bf42e-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bf42e-127">Schema name</span></span>  <br/> |<span data-ttu-id="bf42e-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bf42e-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bf42e-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bf42e-129">Validation file</span></span>  <br/> |<span data-ttu-id="bf42e-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bf42e-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bf42e-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bf42e-131">Can be empty</span></span>  <br/> |<span data-ttu-id="bf42e-132">False</span><span class="sxs-lookup"><span data-stu-id="bf42e-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bf42e-133">См. также</span><span class="sxs-lookup"><span data-stu-id="bf42e-133">See also</span></span>



[<span data-ttu-id="bf42e-134">Операция SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="bf42e-134">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)


- [<span data-ttu-id="bf42e-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bf42e-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

