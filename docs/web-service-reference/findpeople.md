---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'Элемент FindPeople указывает набор данных, используемых в запросе FindPeople. Данные включают ноль или более следующих элементов: фигуру пользователя (необязательно), представление элемента индексированной страницы, ограничение (необязательно), ограничение объединения (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).'
ms.openlocfilehash: 4777601b7146ec857b5c79fa9d4ced59a7247889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462903"
---
# <a name="findpeople"></a><span data-ttu-id="744bf-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="744bf-104">FindPeople</span></span>

<span data-ttu-id="744bf-105">Элемент **FindPeople** указывает набор данных, используемых в запросе FindPeople.</span><span class="sxs-lookup"><span data-stu-id="744bf-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="744bf-106">Данные включают ноль или более следующих элементов: фигуру пользователя (необязательно), представление элемента индексированной страницы, ограничение (необязательно), ограничение объединения (необязательно), порядок сортировки (необязательно), идентификатор родительской папки и строка запроса (необязательно).</span><span class="sxs-lookup"><span data-stu-id="744bf-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
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

 <span data-ttu-id="744bf-107">**финдпеоплетипе**</span><span class="sxs-lookup"><span data-stu-id="744bf-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="744bf-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="744bf-108">Attributes and elements</span></span>

<span data-ttu-id="744bf-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="744bf-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="744bf-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="744bf-110">Attributes</span></span>

<span data-ttu-id="744bf-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="744bf-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="744bf-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="744bf-112">Child elements</span></span>

<span data-ttu-id="744bf-113">[Персонашапе](personashape.md)  |  [Индекседпажеитемвиев](indexedpageitemview.md)  |  [Ограничение](restriction.md)  |  [Аггрегатионрестриктион](aggregationrestriction.md)  |  [SortOrder](sortorder.md)  |  [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md)  |  [Строка запроса (куеристрингтипе)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="744bf-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="744bf-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="744bf-114">Parent elements</span></span>

<span data-ttu-id="744bf-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="744bf-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="744bf-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="744bf-116">Remarks</span></span>

<span data-ttu-id="744bf-117">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="744bf-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="744bf-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="744bf-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="744bf-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="744bf-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="744bf-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="744bf-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="744bf-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="744bf-121">Schema name</span></span>  <br/> |<span data-ttu-id="744bf-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="744bf-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="744bf-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="744bf-123">Validation file</span></span>  <br/> |<span data-ttu-id="744bf-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="744bf-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="744bf-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="744bf-125">Can be empty</span></span>  <br/> |<span data-ttu-id="744bf-126">false</span><span class="sxs-lookup"><span data-stu-id="744bf-126">false</span></span>  <br/> |
   

