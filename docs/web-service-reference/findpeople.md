---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'Элемент FindPeople определяет набор данных, используемые в запросе FindPeople. Данные включают 0 или более из следующих элементов: фигуры пользователя (необязательно), индексируемых элементов страниц, ограничение (необязательно), объединение ограничение (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762589"
---
# <a name="findpeople"></a><span data-ttu-id="ab0ec-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="ab0ec-104">FindPeople</span></span>

<span data-ttu-id="ab0ec-105">Элемент **FindPeople** определяет набор данных, используемые в запросе FindPeople.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="ab0ec-106">Данные включают 0 или более из следующих элементов: фигуры пользователя (необязательно), индексируемых элементов страниц, ограничение (необязательно), объединение ограничение (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).</span><span class="sxs-lookup"><span data-stu-id="ab0ec-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 <span data-ttu-id="ab0ec-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="ab0ec-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab0ec-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ab0ec-108">Attributes and elements</span></span>

<span data-ttu-id="ab0ec-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab0ec-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ab0ec-110">Attributes</span></span>

<span data-ttu-id="ab0ec-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ab0ec-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ab0ec-112">Child elements</span></span>

<span data-ttu-id="ab0ec-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [ограничение](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [ Строка запроса (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="ab0ec-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ab0ec-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ab0ec-114">Parent elements</span></span>

<span data-ttu-id="ab0ec-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ab0ec-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="ab0ec-116">Remarks</span></span>

<span data-ttu-id="ab0ec-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ab0ec-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab0ec-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab0ec-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ab0ec-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab0ec-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ab0ec-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ab0ec-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ab0ec-121">Schema name</span></span>  <br/> |<span data-ttu-id="ab0ec-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ab0ec-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ab0ec-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ab0ec-123">Validation file</span></span>  <br/> |<span data-ttu-id="ab0ec-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ab0ec-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ab0ec-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ab0ec-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ab0ec-126">Нет</span><span class="sxs-lookup"><span data-stu-id="ab0ec-126">false</span></span>  <br/> |
   

