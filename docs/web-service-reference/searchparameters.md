---
title: сеарчпараметерс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SearchParameters
api_type:
- schema
ms.assetid: 34602cb1-dc33-4552-a98c-3e77f614daa3
description: Элемент Сеарчпараметерс представляет параметры, определяющие папку поиска.
ms.openlocfilehash: b534574a1292d78c8df99f5186990b114fc4e70a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835299"
---
# <a name="searchparameters"></a><span data-ttu-id="d67b5-103">сеарчпараметерс</span><span class="sxs-lookup"><span data-stu-id="d67b5-103">SearchParameters</span></span>

<span data-ttu-id="d67b5-104">Элемент **сеарчпараметерс** представляет параметры, определяющие папку поиска.</span><span class="sxs-lookup"><span data-stu-id="d67b5-104">The **SearchParameters** element represents the parameters that define a search folder.</span></span> 
  
```xml
<SearchParameters Traversal="">
   <Restriction/>
   <BaseFolderIds/>
</SearchParameters>
```

 <span data-ttu-id="d67b5-105">**сеарчпараметерстипе**</span><span class="sxs-lookup"><span data-stu-id="d67b5-105">**SearchParametersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d67b5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d67b5-106">Attributes and elements</span></span>

<span data-ttu-id="d67b5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d67b5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d67b5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d67b5-108">Attributes</span></span>

|<span data-ttu-id="d67b5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d67b5-109">**Attribute**</span></span>|<span data-ttu-id="d67b5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d67b5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d67b5-111">**Обход**</span><span class="sxs-lookup"><span data-stu-id="d67b5-111">**Traversal**</span></span> <br/> |<span data-ttu-id="d67b5-112">Описывает, как папка поиска проходит по иерархии папок.</span><span class="sxs-lookup"><span data-stu-id="d67b5-112">Describes how a search folder traverses the folder hierarchy.</span></span> <span data-ttu-id="d67b5-113">Эти параметры предназначены для **глубокого** или неполного **поиска.**</span><span class="sxs-lookup"><span data-stu-id="d67b5-113">The options are for either a **Deep** or a **Shallow** search.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d67b5-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d67b5-114">Child elements</span></span>

|<span data-ttu-id="d67b5-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d67b5-115">**Element**</span></span>|<span data-ttu-id="d67b5-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d67b5-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d67b5-117">Restriction</span><span class="sxs-lookup"><span data-stu-id="d67b5-117">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="d67b5-118">Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.</span><span class="sxs-lookup"><span data-stu-id="d67b5-118">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="d67b5-119">басефолдеридс</span><span class="sxs-lookup"><span data-stu-id="d67b5-119">BaseFolderIds</span></span>](basefolderids.md) <br/> |<span data-ttu-id="d67b5-120">Представляет коллекцию папок, которые будут mined для определения содержимого папки поиска.</span><span class="sxs-lookup"><span data-stu-id="d67b5-120">Represents the collection of folders that will be mined to determine the contents of a search folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d67b5-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d67b5-121">Parent elements</span></span>

|<span data-ttu-id="d67b5-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d67b5-122">**Element**</span></span>|<span data-ttu-id="d67b5-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d67b5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d67b5-124">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d67b5-124">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d67b5-125">Представляет папку поиска, содержащуюся в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d67b5-125">Represents a search folder that is contained in a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d67b5-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="d67b5-126">Remarks</span></span>

<span data-ttu-id="d67b5-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d67b5-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d67b5-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d67b5-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d67b5-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d67b5-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d67b5-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d67b5-130">Schema Name</span></span>  <br/> |<span data-ttu-id="d67b5-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d67b5-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="d67b5-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d67b5-132">Validation File</span></span>  <br/> |<span data-ttu-id="d67b5-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d67b5-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d67b5-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d67b5-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="d67b5-135">False</span><span class="sxs-lookup"><span data-stu-id="d67b5-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d67b5-136">См. также</span><span class="sxs-lookup"><span data-stu-id="d67b5-136">See also</span></span>



- [<span data-ttu-id="d67b5-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d67b5-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

