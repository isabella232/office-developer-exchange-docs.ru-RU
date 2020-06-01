---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: Элемент SyncFolderItems определяет запрос на синхронизацию элементов в папке хранилища Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465151"
---
# <a name="syncfolderitems"></a><span data-ttu-id="d773a-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="d773a-103">SyncFolderItems</span></span>

<span data-ttu-id="d773a-104">Элемент **SyncFolderItems** определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d773a-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="d773a-105">**синкфолдеритемстипе**</span><span class="sxs-lookup"><span data-stu-id="d773a-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d773a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d773a-106">Attributes and elements</span></span>

<span data-ttu-id="d773a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d773a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d773a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d773a-108">Attributes</span></span>

<span data-ttu-id="d773a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d773a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d773a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d773a-110">Child elements</span></span>

|<span data-ttu-id="d773a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d773a-111">**Element**</span></span>|<span data-ttu-id="d773a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d773a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d773a-113">итемшапе</span><span class="sxs-lookup"><span data-stu-id="d773a-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="d773a-114">Определяет свойства и контент элемента, включаемые в ответ SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="d773a-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="d773a-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d773a-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d773a-116">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="d773a-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="d773a-117">Представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="d773a-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="d773a-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d773a-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d773a-119">синкстате</span><span class="sxs-lookup"><span data-stu-id="d773a-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d773a-120">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="d773a-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="d773a-121">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d773a-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="d773a-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d773a-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d773a-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="d773a-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="d773a-124">Определяет элементы, которые необходимо пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d773a-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="d773a-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d773a-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d773a-126">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="d773a-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="d773a-127">Описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d773a-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="d773a-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="d773a-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="d773a-129">синкскопе</span><span class="sxs-lookup"><span data-stu-id="d773a-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="d773a-130">Указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой и сведениями о них.</span><span class="sxs-lookup"><span data-stu-id="d773a-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="d773a-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="d773a-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d773a-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d773a-132">Parent elements</span></span>

<span data-ttu-id="d773a-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="d773a-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d773a-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="d773a-134">Remarks</span></span>

<span data-ttu-id="d773a-135">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d773a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d773a-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d773a-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d773a-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d773a-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d773a-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d773a-138">Schema name</span></span>  <br/> |<span data-ttu-id="d773a-139">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="d773a-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="d773a-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d773a-140">Validation file</span></span>  <br/> |<span data-ttu-id="d773a-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d773a-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d773a-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d773a-142">Can be empty</span></span>  <br/> |<span data-ttu-id="d773a-143">False</span><span class="sxs-lookup"><span data-stu-id="d773a-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d773a-144">См. также</span><span class="sxs-lookup"><span data-stu-id="d773a-144">See also</span></span>



[<span data-ttu-id="d773a-145">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="d773a-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="d773a-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d773a-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

