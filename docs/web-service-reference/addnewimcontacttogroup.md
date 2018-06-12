---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: Элемент AddNewImContactToGroup определяет запрос на добавление нового мгновенного обмена сообщениями контакта в группу мгновенного обмена сообщениями.
ms.openlocfilehash: 2736bac6880a11101e9bffee12033c838705700e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761348"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="83a94-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="83a94-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="83a94-104">Элемент **AddNewImContactToGroup** определяет запрос на добавление нового мгновенного обмена сообщениями контакта в группу мгновенного обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="83a94-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="83a94-105">**AddNewImContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="83a94-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83a94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="83a94-106">Attributes and elements</span></span>

<span data-ttu-id="83a94-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="83a94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83a94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="83a94-108">Attributes</span></span>

<span data-ttu-id="83a94-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="83a94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83a94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="83a94-110">Child elements</span></span>

<span data-ttu-id="83a94-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="83a94-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83a94-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="83a94-112">Parent elements</span></span>

<span data-ttu-id="83a94-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="83a94-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83a94-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="83a94-114">Remarks</span></span>

<span data-ttu-id="83a94-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="83a94-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="83a94-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="83a94-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83a94-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="83a94-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83a94-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="83a94-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83a94-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="83a94-119">Schema name</span></span>  <br/> |<span data-ttu-id="83a94-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="83a94-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83a94-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="83a94-121">Validation file</span></span>  <br/> |<span data-ttu-id="83a94-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="83a94-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83a94-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="83a94-123">Can be empty</span></span>  <br/> |<span data-ttu-id="83a94-124">Нет</span><span class="sxs-lookup"><span data-stu-id="83a94-124">false</span></span>  <br/> |
   
