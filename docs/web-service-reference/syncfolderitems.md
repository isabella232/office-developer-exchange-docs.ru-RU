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
description: Элемент SyncFolderItems определяет запрос для синхронизации элементов в папке хранилища Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840126"
---
# <a name="syncfolderitems"></a><span data-ttu-id="8c680-103">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="8c680-103">SyncFolderItems</span></span>

<span data-ttu-id="8c680-104">Элемент **SyncFolderItems** определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="8c680-104">The **SyncFolderItems** element defines a request to synchronize items in an Exchange store folder.</span></span> 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 <span data-ttu-id="8c680-105">**SyncFolderItemsType**</span><span class="sxs-lookup"><span data-stu-id="8c680-105">**SyncFolderItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8c680-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8c680-106">Attributes and elements</span></span>

<span data-ttu-id="8c680-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8c680-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8c680-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8c680-108">Attributes</span></span>

<span data-ttu-id="8c680-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c680-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8c680-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8c680-110">Child elements</span></span>

|<span data-ttu-id="8c680-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8c680-111">**Element**</span></span>|<span data-ttu-id="8c680-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8c680-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8c680-113">ItemShape</span><span class="sxs-lookup"><span data-stu-id="8c680-113">ItemShape</span></span>](itemshape.md) <br/> |<span data-ttu-id="8c680-114">Определяет свойства элемента и содержимого для включения в SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="8c680-114">Identifies the item properties and content to include in a SyncFolderItems response.</span></span> <span data-ttu-id="8c680-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c680-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8c680-116">SyncFolderId</span><span class="sxs-lookup"><span data-stu-id="8c680-116">SyncFolderId</span></span>](syncfolderid.md) <br/> |<span data-ttu-id="8c680-117">Представляет папку, содержащую элементы для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8c680-117">Represents the folder that contains the items to synchronize.</span></span> <span data-ttu-id="8c680-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c680-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8c680-119">Состояние</span><span class="sxs-lookup"><span data-stu-id="8c680-119">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8c680-120">Содержит формы кодировки Base64 данных синхронизации, который обновляется после каждого успешного запроса.</span><span class="sxs-lookup"><span data-stu-id="8c680-120">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="8c680-121">Используется для определения состояния синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8c680-121">This is used to identify the synchronization state.</span></span> <span data-ttu-id="8c680-122">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8c680-122">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8c680-123">Пропуск</span><span class="sxs-lookup"><span data-stu-id="8c680-123">Ignore</span></span>](ignore.md) <br/> |<span data-ttu-id="8c680-124">Определяет элементы, чтобы пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8c680-124">Identifies items to skip during synchronization.</span></span> <span data-ttu-id="8c680-125">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8c680-125">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8c680-126">MaxChangesReturned</span><span class="sxs-lookup"><span data-stu-id="8c680-126">MaxChangesReturned</span></span>](maxchangesreturned.md) <br/> |<span data-ttu-id="8c680-127">Описывает максимальное число изменений, которые могут возвращаться в ответ синхронизации.</span><span class="sxs-lookup"><span data-stu-id="8c680-127">Describes the maximum number of changes that can be returned in a synchronization response.</span></span> <span data-ttu-id="8c680-128">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c680-128">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="8c680-129">SyncScope</span><span class="sxs-lookup"><span data-stu-id="8c680-129">SyncScope</span></span>](syncscope.md) <br/> |<span data-ttu-id="8c680-130">Указывает, будет ли только что элементов или элементы и сведения, папки, связанной возвращаются в синхронизации ответа.</span><span class="sxs-lookup"><span data-stu-id="8c680-130">Specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> <span data-ttu-id="8c680-131">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8c680-131">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8c680-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8c680-132">Parent elements</span></span>

<span data-ttu-id="8c680-133">Нет.</span><span class="sxs-lookup"><span data-stu-id="8c680-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8c680-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="8c680-134">Remarks</span></span>

<span data-ttu-id="8c680-135">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8c680-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8c680-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8c680-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8c680-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8c680-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8c680-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8c680-138">Schema name</span></span>  <br/> |<span data-ttu-id="8c680-139">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="8c680-139">messages schema</span></span>  <br/> |
|<span data-ttu-id="8c680-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8c680-140">Validation file</span></span>  <br/> |<span data-ttu-id="8c680-141">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8c680-141">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8c680-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8c680-142">Can be empty</span></span>  <br/> |<span data-ttu-id="8c680-143">False</span><span class="sxs-lookup"><span data-stu-id="8c680-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8c680-144">См. также</span><span class="sxs-lookup"><span data-stu-id="8c680-144">See also</span></span>



[<span data-ttu-id="8c680-145">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="8c680-145">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="8c680-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8c680-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

