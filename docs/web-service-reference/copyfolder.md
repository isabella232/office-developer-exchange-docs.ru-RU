---
title: CopyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: 7d5cd08a-fe81-4cb6-a5a0-6dec2d3c93d4
description: Элемент CopyFolder определяет запрос для копирования папки почтового ящика в хранилище Exchange.
ms.openlocfilehash: 7bcfcc7f4212b3a3bd339fa5863df2990eb20d6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761838"
---
# <a name="copyfolder"></a><span data-ttu-id="8324d-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="8324d-103">CopyFolder</span></span>

<span data-ttu-id="8324d-104">Элемент **CopyFolder** определяет запрос для копирования папки почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="8324d-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="8324d-105">**CopyFolderType**</span><span class="sxs-lookup"><span data-stu-id="8324d-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8324d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8324d-106">Attributes and elements</span></span>

<span data-ttu-id="8324d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8324d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8324d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8324d-108">Attributes</span></span>

<span data-ttu-id="8324d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8324d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8324d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8324d-110">Child elements</span></span>

|<span data-ttu-id="8324d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8324d-111">**Element**</span></span>|<span data-ttu-id="8324d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8324d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8324d-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="8324d-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="8324d-114">Представляет конечной папки для скопированной папке.</span><span class="sxs-lookup"><span data-stu-id="8324d-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="8324d-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="8324d-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="8324d-116">Содержит набор папок, которые следует скопировать в папку, указанную в элементе [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="8324d-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8324d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8324d-117">Parent elements</span></span>

<span data-ttu-id="8324d-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="8324d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8324d-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="8324d-119">Remarks</span></span>

<span data-ttu-id="8324d-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8324d-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8324d-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8324d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8324d-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8324d-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8324d-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8324d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8324d-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8324d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8324d-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8324d-125">Validation File</span></span>  <br/> |<span data-ttu-id="8324d-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8324d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8324d-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8324d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8324d-128">False</span><span class="sxs-lookup"><span data-stu-id="8324d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8324d-129">См. также</span><span class="sxs-lookup"><span data-stu-id="8324d-129">See also</span></span>



[<span data-ttu-id="8324d-130">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="8324d-130">CopyFolder operation</span></span>](copyfolder-operation.md)

