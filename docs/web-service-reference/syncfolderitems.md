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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465151"
---
# <a name="syncfolderitems"></a><span data-ttu-id="7a905-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7a905-103">SyncFolderItems</span></span>

<span data-ttu-id="7a905-104">Элемент **SyncFolderItems** определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a905-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="7a905-105">**синкфолдеритемстипе**</span><span class="sxs-lookup"><span data-stu-id="7a905-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a905-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a905-106">Attributes and elements</span></span>

<span data-ttu-id="7a905-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7a905-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a905-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a905-108">Attributes</span></span>

<span data-ttu-id="7a905-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7a905-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a905-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a905-110">Child elements</span></span>

|<span data-ttu-id="7a905-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a905-111">**Element**</span></span>|<span data-ttu-id="7a905-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a905-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a905-113">итемшапе</span><span class="sxs-lookup"><span data-stu-id="7a905-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="7a905-114">Определяет свойства и контент элемента, включаемые в ответ SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="7a905-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="7a905-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a905-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a905-116">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="7a905-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="7a905-117">Представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="7a905-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="7a905-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a905-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a905-119">синкстате</span><span class="sxs-lookup"><span data-stu-id="7a905-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7a905-120">Содержит форму синхронизации данных с кодировкой base64, которая обновляется после каждого успешного выполнения запроса.</span><span class="sxs-lookup"><span data-stu-id="7a905-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="7a905-121">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7a905-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="7a905-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7a905-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7a905-123">Ignore</span><span class="sxs-lookup"><span data-stu-id="7a905-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="7a905-124">Определяет элементы, которые необходимо пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7a905-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="7a905-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7a905-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="7a905-126">максчанжесретурнед</span><span class="sxs-lookup"><span data-stu-id="7a905-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="7a905-127">Описывает максимальное число изменений, которые могут быть возвращены в ответе синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7a905-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="7a905-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a905-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a905-129">синкскопе</span><span class="sxs-lookup"><span data-stu-id="7a905-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="7a905-130">Указывает, будут ли в ответе синхронизации возвращаться только элементы, связанные с папкой и сведениями о них.</span><span class="sxs-lookup"><span data-stu-id="7a905-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="7a905-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7a905-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a905-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a905-132">Parent elements</span></span>

<span data-ttu-id="7a905-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a905-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a905-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="7a905-134">Remarks</span></span>

<span data-ttu-id="7a905-135">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7a905-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a905-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a905-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a905-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a905-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a905-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a905-138">Schema name</span></span>  <br/> |<span data-ttu-id="7a905-139">схема сообщений</span><span class="sxs-lookup"><span data-stu-id="7a905-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="7a905-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a905-140">Validation file</span></span>  <br/> |<span data-ttu-id="7a905-141">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7a905-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a905-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a905-142">Can be empty</span></span>  <br/> |<span data-ttu-id="7a905-143">False</span><span class="sxs-lookup"><span data-stu-id="7a905-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a905-144">См. также</span><span class="sxs-lookup"><span data-stu-id="7a905-144">See also</span></span>



[<span data-ttu-id="7a905-145">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7a905-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="7a905-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7a905-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

