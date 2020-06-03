---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: Элемент GroupId однозначно идентифицирует группу.
ms.openlocfilehash: 3b8de4d0fef95e2caff4db0d90bb303830022d36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530094"
---
# <a name="groupid"></a><span data-ttu-id="bddf3-103">GroupId</span><span class="sxs-lookup"><span data-stu-id="bddf3-103">GroupId</span></span>

<span data-ttu-id="bddf3-104">Элемент **groupId** однозначно идентифицирует группу.</span><span class="sxs-lookup"><span data-stu-id="bddf3-104">The **GroupId** element uniquely identifies a group.</span></span> 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 <span data-ttu-id="bddf3-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="bddf3-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bddf3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bddf3-106">Attributes and elements</span></span>

<span data-ttu-id="bddf3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bddf3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bddf3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bddf3-108">Attributes</span></span>

|<span data-ttu-id="bddf3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bddf3-109">**Attribute**</span></span>|<span data-ttu-id="bddf3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bddf3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bddf3-111">Id</span><span class="sxs-lookup"><span data-stu-id="bddf3-111">Id</span></span>  <br/> |<span data-ttu-id="bddf3-112">Текстовое значение атрибута **ID** — идентификатор группы.</span><span class="sxs-lookup"><span data-stu-id="bddf3-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="bddf3-113">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="bddf3-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="bddf3-114">Текстовое значение атрибута **чанжекэй** — это ключ изменения группы.</span><span class="sxs-lookup"><span data-stu-id="bddf3-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bddf3-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bddf3-115">Child elements</span></span>

<span data-ttu-id="bddf3-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bddf3-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bddf3-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bddf3-117">Parent elements</span></span>

<span data-ttu-id="bddf3-118">[AddNewImContactToGroup](addnewimcontacttogroup.md)  |  [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md)  |  [AddImContactToGroup](addimcontacttogroup.md)  |  [RemoveContactFromImList](removecontactfromimlist.md)  |  [RemoveImContactFromGroup](removeimcontactfromgroup.md)  |  [RemoveImGroup](removeimgroup.md)  |  [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)  |  [SetImGroup](setimgroup.md)</span><span class="sxs-lookup"><span data-stu-id="bddf3-118">[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md) | [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bddf3-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="bddf3-119">Remarks</span></span>

<span data-ttu-id="bddf3-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bddf3-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="bddf3-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bddf3-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bddf3-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bddf3-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bddf3-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bddf3-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bddf3-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bddf3-124">Schema name</span></span>  <br/> |<span data-ttu-id="bddf3-125">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bddf3-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bddf3-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bddf3-126">Validation file</span></span>  <br/> |<span data-ttu-id="bddf3-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bddf3-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bddf3-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bddf3-128">Can be empty</span></span>  <br/> ||
   

