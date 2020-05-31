---
title: инклудеунсеарчаблеитемс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: Элемент Инклудеунсеарчаблеитемс указывает, следует ли включать элементы, поиск которых невозможен.
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833907"
---
# <a name="includeunsearchableitems"></a><span data-ttu-id="f4e37-103">инклудеунсеарчаблеитемс</span><span class="sxs-lookup"><span data-stu-id="f4e37-103">IncludeUnsearchableItems</span></span>

<span data-ttu-id="f4e37-104">Элемент **инклудеунсеарчаблеитемс** указывает, следует ли включать элементы, поиск которых невозможен.</span><span class="sxs-lookup"><span data-stu-id="f4e37-104">The **IncludeUnsearchableItems** element specifies whether to include items that cannot be searched.</span></span> 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
```

 <span data-ttu-id="f4e37-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f4e37-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4e37-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f4e37-106">Attributes and elements</span></span>

<span data-ttu-id="f4e37-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f4e37-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4e37-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f4e37-108">Attributes</span></span>

<span data-ttu-id="f4e37-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4e37-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4e37-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f4e37-110">Child elements</span></span>

<span data-ttu-id="f4e37-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="f4e37-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4e37-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f4e37-112">Parent elements</span></span>

|<span data-ttu-id="f4e37-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f4e37-113">**Element**</span></span>|<span data-ttu-id="f4e37-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f4e37-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4e37-115">финдмаилбоксстатистиксбикэйвордс</span><span class="sxs-lookup"><span data-stu-id="f4e37-115">FindMailboxStatisticsByKeywords</span></span>](findmailboxstatisticsbykeywords.md) <br/> |<span data-ttu-id="f4e37-116">Указывает запрос на поиск статистики почтовых ящиков по ключевому слову.</span><span class="sxs-lookup"><span data-stu-id="f4e37-116">Specifies a request to search for mailbox statistics by keyword.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4e37-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f4e37-117">Text value</span></span>

<span data-ttu-id="f4e37-118">Текстовое значение **true** для элемента **инклудеунсеарчаблеитемс** указывает на то, что статистика не включается для элементов, которые не могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4e37-118">A text value of **true** for the **IncludeUnsearchableItems** element indicates that statistics are not included for items that are not searchable.</span></span> <span data-ttu-id="f4e37-119">Значение **false** указывает, что статистика включена для элементов, которые не могут быть доступны для поиска.</span><span class="sxs-lookup"><span data-stu-id="f4e37-119">A value of **false** indicates that statistics are included for items that are not searchable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f4e37-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="f4e37-120">Remarks</span></span>

<span data-ttu-id="f4e37-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f4e37-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f4e37-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4e37-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4e37-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f4e37-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4e37-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f4e37-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f4e37-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f4e37-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f4e37-126">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="f4e37-126">Message schema</span></span>  <br/> |
|<span data-ttu-id="f4e37-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f4e37-127">Validation File</span></span>  <br/> |<span data-ttu-id="f4e37-128">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f4e37-128">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f4e37-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f4e37-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f4e37-130">См. также</span><span class="sxs-lookup"><span data-stu-id="f4e37-130">See also</span></span>



- [<span data-ttu-id="f4e37-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f4e37-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

