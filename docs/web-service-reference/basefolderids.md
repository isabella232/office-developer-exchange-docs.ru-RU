---
title: BaseFolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: Элемент BaseFolderIds представляет коллекцию папок, которые будут получены для определения содержимого папки поиска.
ms.openlocfilehash: 960e4d9c1d6eb37bf988bf163e696cbba3e1ef6f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761540"
---
# <a name="basefolderids"></a><span data-ttu-id="8b6aa-103">BaseFolderIds</span><span class="sxs-lookup"><span data-stu-id="8b6aa-103">BaseFolderIds</span></span>

<span data-ttu-id="8b6aa-104">Элемент **BaseFolderIds** представляет коллекцию папок, которые будут получены для определения содержимого папки поиска.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="8b6aa-105">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="8b6aa-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b6aa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b6aa-106">Attributes and elements</span></span>

<span data-ttu-id="8b6aa-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b6aa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b6aa-108">Attributes</span></span>

<span data-ttu-id="8b6aa-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b6aa-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b6aa-110">Child elements</span></span>

|<span data-ttu-id="8b6aa-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b6aa-111">**Element**</span></span>|<span data-ttu-id="8b6aa-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b6aa-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b6aa-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="8b6aa-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="8b6aa-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="8b6aa-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8b6aa-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="8b6aa-116">Идентифицирует MicrosoftExchange Server 2007 папок, которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b6aa-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b6aa-117">Parent elements</span></span>

|<span data-ttu-id="8b6aa-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b6aa-118">**Element**</span></span>|<span data-ttu-id="8b6aa-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b6aa-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b6aa-120">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="8b6aa-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="8b6aa-121">Представляет параметры, определяющие папки поиска.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8b6aa-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b6aa-122">Remarks</span></span>

<span data-ttu-id="8b6aa-123">Элемент **BaseFolderIds** должен содержать по крайней мере один элемент [FolderId](folderid.md) или [DistinguishedFolderId](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="8b6aa-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="8b6aa-124">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8b6aa-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b6aa-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b6aa-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b6aa-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b6aa-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b6aa-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b6aa-127">Schema name</span></span>  <br/> |<span data-ttu-id="8b6aa-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8b6aa-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b6aa-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b6aa-129">Validation file</span></span>  <br/> |<span data-ttu-id="8b6aa-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8b6aa-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b6aa-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b6aa-131">Can be empty</span></span>  <br/> |<span data-ttu-id="8b6aa-132">False</span><span class="sxs-lookup"><span data-stu-id="8b6aa-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b6aa-133">См. также</span><span class="sxs-lookup"><span data-stu-id="8b6aa-133">See also</span></span>



- [<span data-ttu-id="8b6aa-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b6aa-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

