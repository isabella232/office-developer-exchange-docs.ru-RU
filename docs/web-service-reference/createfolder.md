---
title: CreateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 110bada1-517b-4bd6-870d-7086dc879e5d
description: Элемент CreateFolder определяет запрос на создание папки в хранилище Exchange.
ms.openlocfilehash: e30af23b8ed8669053b94be460d62fbf7abf24c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19761869"
---
# <a name="createfolder"></a><span data-ttu-id="eed71-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="eed71-103">CreateFolder</span></span>

<span data-ttu-id="eed71-104">Элемент **CreateFolder** определяет запрос на создание папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="eed71-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="eed71-105">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="eed71-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eed71-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eed71-106">Attributes and elements</span></span>

<span data-ttu-id="eed71-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eed71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eed71-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eed71-108">Attributes</span></span>

<span data-ttu-id="eed71-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="eed71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eed71-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eed71-110">Child elements</span></span>

|<span data-ttu-id="eed71-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eed71-111">**Element**</span></span>|<span data-ttu-id="eed71-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eed71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eed71-113">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="eed71-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="eed71-114">Элемент, определяющий расположение, где будет создана новая папка.</span><span class="sxs-lookup"><span data-stu-id="eed71-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="eed71-115">Папки</span><span class="sxs-lookup"><span data-stu-id="eed71-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="eed71-116">Элемент, содержащий все папках для создания.</span><span class="sxs-lookup"><span data-stu-id="eed71-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eed71-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eed71-117">Parent elements</span></span>

<span data-ttu-id="eed71-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="eed71-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eed71-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="eed71-119">Remarks</span></span>

<span data-ttu-id="eed71-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="eed71-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eed71-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eed71-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eed71-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eed71-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eed71-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eed71-123">Schema Name</span></span>  <br/> |<span data-ttu-id="eed71-124">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="eed71-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="eed71-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eed71-125">Validation File</span></span>  <br/> |<span data-ttu-id="eed71-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eed71-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eed71-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eed71-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="eed71-128">False</span><span class="sxs-lookup"><span data-stu-id="eed71-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eed71-129">См. также</span><span class="sxs-lookup"><span data-stu-id="eed71-129">See also</span></span>



[<span data-ttu-id="eed71-130">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="eed71-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="eed71-131">Создание папки (веб-служб Exchange)</span><span class="sxs-lookup"><span data-stu-id="eed71-131">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

