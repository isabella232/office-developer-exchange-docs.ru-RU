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
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840126"
---
# <a name="syncfolderitems"></a><span data-ttu-id="a1c89-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a1c89-103">SyncFolderItems</span></span>

<span data-ttu-id="a1c89-104">Элемент **SyncFolderItems** определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a1c89-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="a1c89-105">**синкфолдеритемстипе**</span><span class="sxs-lookup"><span data-stu-id="a1c89-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1c89-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1c89-106">Attributes and elements</span></span>

<span data-ttu-id="a1c89-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1c89-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1c89-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1c89-108">Attributes</span></span>

<span data-ttu-id="a1c89-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1c89-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1c89-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1c89-110">Child elements</span></span>

|<span data-ttu-id="a1c89-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1c89-111">**Element**</span></span>|<span data-ttu-id="a1c89-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1c89-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1c89-113">итемшапе</span><span class="sxs-lookup"><span data-stu-id="a1c89-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="a1c89-114">Определяет свойства и контент элемента, включаемые в ответ SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="a1c89-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="a1c89-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c89-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a1c89-116">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="a1c89-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="a1c89-117">Представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="a1c89-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="a1c89-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c89-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a1c89-119">синкстате</span><span class="sxs-lookup"><span data-stu-id="a1c89-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a1c89-120">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="a1c89-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="a1c89-121">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a1c89-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="a1c89-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a1c89-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a1c89-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="a1c89-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="a1c89-124">Определяет элементы, которые необходимо пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a1c89-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="a1c89-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a1c89-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="a1c89-126">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="a1c89-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="a1c89-127">Описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a1c89-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="a1c89-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="a1c89-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="a1c89-129">синкскопе</span><span class="sxs-lookup"><span data-stu-id="a1c89-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="a1c89-130">Указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой и сведениями о них.</span><span class="sxs-lookup"><span data-stu-id="a1c89-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="a1c89-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="a1c89-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1c89-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1c89-132">Parent elements</span></span>

<span data-ttu-id="a1c89-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1c89-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1c89-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1c89-134">Remarks</span></span>

<span data-ttu-id="a1c89-135">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1c89-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1c89-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1c89-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1c89-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1c89-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1c89-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1c89-138">Schema name</span></span>  <br/> |<span data-ttu-id="a1c89-139">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="a1c89-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="a1c89-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1c89-140">Validation file</span></span>  <br/> |<span data-ttu-id="a1c89-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a1c89-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1c89-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1c89-142">Can be empty</span></span>  <br/> |<span data-ttu-id="a1c89-143">False</span><span class="sxs-lookup"><span data-stu-id="a1c89-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1c89-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a1c89-144">See also</span></span>



[<span data-ttu-id="a1c89-145">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="a1c89-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="a1c89-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1c89-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

