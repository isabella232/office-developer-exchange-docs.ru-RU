---
title: ImItemList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 556457d5-a730-4131-853f-1198c27c5942
description: Элемент ImItemList содержит список групп мгновенного обмена сообщениями и обмена мгновенными сообщениями.
ms.openlocfilehash: 490ac57da0c7ae7bedc75e94b7e21dc30c9da23f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833896"
---
# <a name="imitemlist"></a><span data-ttu-id="fdc6b-103">ImItemList</span><span class="sxs-lookup"><span data-stu-id="fdc6b-103">ImItemList</span></span>

<span data-ttu-id="fdc6b-104">Элемент **ImItemList** содержит список групп мгновенного обмена сообщениями и обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fdc6b-104">The **ImItemList** element contains a list of instant messaging groups and instant messaging contacts.</span></span> 
  
```XML
<ImItemList>
   <Groups/>
   <Personas/>
</ImItemList>
```

 <span data-ttu-id="fdc6b-105">**ImItemListType**</span><span class="sxs-lookup"><span data-stu-id="fdc6b-105">**ImItemListType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdc6b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fdc6b-106">Attributes and elements</span></span>

<span data-ttu-id="fdc6b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fdc6b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdc6b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fdc6b-108">Attributes</span></span>

<span data-ttu-id="fdc6b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="fdc6b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fdc6b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fdc6b-110">Child elements</span></span>

<span data-ttu-id="fdc6b-111">[Группы (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [пользователей](personas-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="fdc6b-111">[Groups (ArrayOfImGroupType)](groups-arrayofimgrouptype.md) | [Personas](personas-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fdc6b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fdc6b-112">Parent elements</span></span>

<span data-ttu-id="fdc6b-113">[GetImItemsResponse](getimitemsresponse.md) | [GetImItemListResponse](getimitemlistresponse.md)</span><span class="sxs-lookup"><span data-stu-id="fdc6b-113">[GetImItemsResponse](getimitemsresponse.md) | [GetImItemListResponse](getimitemlistresponse.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fdc6b-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="fdc6b-114">Remarks</span></span>

<span data-ttu-id="fdc6b-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="fdc6b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fdc6b-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdc6b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdc6b-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fdc6b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdc6b-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fdc6b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fdc6b-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fdc6b-119">Schema name</span></span>  <br/> |<span data-ttu-id="fdc6b-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fdc6b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fdc6b-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fdc6b-121">Validation file</span></span>  <br/> |<span data-ttu-id="fdc6b-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fdc6b-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fdc6b-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fdc6b-123">Can be empty</span></span>  <br/> ||
   
