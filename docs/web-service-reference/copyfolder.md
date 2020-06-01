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
description: Элемент CopyFolder определяет запрос на копирование папок в почтовом ящике в хранилище Exchange.
ms.openlocfilehash: fa75272540169a96d5567181d27b8a8f056cce42
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452512"
---
# <a name="copyfolder"></a><span data-ttu-id="f3571-103">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="f3571-103">CopyFolder</span></span>

<span data-ttu-id="f3571-104">Элемент **CopyFolder** определяет запрос на копирование папок в почтовом ящике в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3571-104">The **CopyFolder** element defines a request to copy folders in a mailbox in the Exchange store.</span></span> 
  
```xml
<CopyFolder>
   <ToFolderId/>
   <FolderIds/>
</CopyFolder>
```

 <span data-ttu-id="f3571-105">**копифолдертипе**</span><span class="sxs-lookup"><span data-stu-id="f3571-105">**CopyFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3571-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3571-106">Attributes and elements</span></span>

<span data-ttu-id="f3571-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3571-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3571-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3571-108">Attributes</span></span>

<span data-ttu-id="f3571-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f3571-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3571-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3571-110">Child elements</span></span>

|<span data-ttu-id="f3571-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3571-111">**Element**</span></span>|<span data-ttu-id="f3571-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3571-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3571-113">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="f3571-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="f3571-114">Представляет папку назначения для скопированной папки.</span><span class="sxs-lookup"><span data-stu-id="f3571-114">Represents the destination folder for a copied folder.</span></span>  <br/> |
|[<span data-ttu-id="f3571-115">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="f3571-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="f3571-116">Содержит массив папок, которые необходимо скопировать в папку, определяемую элементом [тофолдерид](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f3571-116">Contains an array of folders to copy to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3571-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3571-117">Parent elements</span></span>

<span data-ttu-id="f3571-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3571-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3571-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3571-119">Remarks</span></span>

<span data-ttu-id="f3571-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f3571-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3571-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3571-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3571-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3571-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3571-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3571-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f3571-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3571-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3571-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3571-125">Validation File</span></span>  <br/> |<span data-ttu-id="f3571-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3571-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3571-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3571-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3571-128">False</span><span class="sxs-lookup"><span data-stu-id="f3571-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3571-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f3571-129">See also</span></span>



[<span data-ttu-id="f3571-130">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="f3571-130">CopyFolder operation</span></span>](copyfolder-operation.md)

