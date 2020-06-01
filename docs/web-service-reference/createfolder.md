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
ms.openlocfilehash: c2a971a6b827553a1632c2a86e4d36e3b83a2de3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457545"
---
# <a name="createfolder"></a><span data-ttu-id="757a9-103">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="757a9-103">CreateFolder</span></span>

<span data-ttu-id="757a9-104">Элемент **CreateFolder** определяет запрос на создание папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="757a9-104">The **CreateFolder** element defines a request to create a folder in the Exchange store.</span></span> 
  
```xml
<CreateFolder>
   <ParentFolderId/>
   <Folders/>
</CreateFolder>
```

 <span data-ttu-id="757a9-105">**креатефолдертипе**</span><span class="sxs-lookup"><span data-stu-id="757a9-105">**CreateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="757a9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="757a9-106">Attributes and elements</span></span>

<span data-ttu-id="757a9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="757a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="757a9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="757a9-108">Attributes</span></span>

<span data-ttu-id="757a9-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="757a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="757a9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="757a9-110">Child elements</span></span>

|<span data-ttu-id="757a9-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="757a9-111">**Element**</span></span>|<span data-ttu-id="757a9-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="757a9-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="757a9-113">ParentFolderId (Таржетфолдеридтипе)</span><span class="sxs-lookup"><span data-stu-id="757a9-113">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md) <br/> |<span data-ttu-id="757a9-114">Элемент, определяющий расположение, в котором создается новая папка.</span><span class="sxs-lookup"><span data-stu-id="757a9-114">The element that identifies the location where the new folder is created.</span></span>  <br/> |
|[<span data-ttu-id="757a9-115">Folders</span><span class="sxs-lookup"><span data-stu-id="757a9-115">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="757a9-116">Элемент, содержащий все создаваемые папки.</span><span class="sxs-lookup"><span data-stu-id="757a9-116">The element that contains all the folders to create.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="757a9-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="757a9-117">Parent elements</span></span>

<span data-ttu-id="757a9-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="757a9-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="757a9-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="757a9-119">Remarks</span></span>

<span data-ttu-id="757a9-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="757a9-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="757a9-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="757a9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="757a9-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="757a9-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="757a9-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="757a9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="757a9-124">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="757a9-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="757a9-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="757a9-125">Validation File</span></span>  <br/> |<span data-ttu-id="757a9-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="757a9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="757a9-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="757a9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="757a9-128">False</span><span class="sxs-lookup"><span data-stu-id="757a9-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="757a9-129">См. также</span><span class="sxs-lookup"><span data-stu-id="757a9-129">See also</span></span>



[<span data-ttu-id="757a9-130">Операция CreateFolder</span><span class="sxs-lookup"><span data-stu-id="757a9-130">CreateFolder operation</span></span>](createfolder-operation.md)


[<span data-ttu-id="757a9-131">Создание папок (веб-службы Exchange)</span><span class="sxs-lookup"><span data-stu-id="757a9-131">Creating Folders (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

