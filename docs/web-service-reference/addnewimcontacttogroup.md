---
title: AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d5913619-0c13-429d-b9d2-057e8af220f1
description: Элемент AddNewImContactToGroup определяет запрос на добавление нового контакта для обмена мгновенными сообщениями в группу мгновенных сообщений.
ms.openlocfilehash: c493ba81b23832a462acd425eb60297801f8768f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463652"
---
# <a name="addnewimcontacttogroup"></a><span data-ttu-id="d8dae-103">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="d8dae-103">AddNewImContactToGroup</span></span>

<span data-ttu-id="d8dae-104">Элемент **AddNewImContactToGroup** определяет запрос на добавление нового контакта для обмена мгновенными сообщениями в группу мгновенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="d8dae-104">The **AddNewImContactToGroup** element defines a request to add a new instant messaging contact to an instant messaging group.</span></span> 
  
```XML
<AddNewImContactToGroup>
   <ImAddress/>
   <DisplayName/>
   <GroupId/>
</AddNewImContactToGroup>
```

 <span data-ttu-id="d8dae-105">**аддневимконтакттограуптипе**</span><span class="sxs-lookup"><span data-stu-id="d8dae-105">**AddNewImContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8dae-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d8dae-106">Attributes and elements</span></span>

<span data-ttu-id="d8dae-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d8dae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8dae-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d8dae-108">Attributes</span></span>

<span data-ttu-id="d8dae-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d8dae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8dae-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d8dae-110">Child elements</span></span>

<span data-ttu-id="d8dae-111">[Адрес (нонемптистрингтипе)](imaddress-nonemptystringtype.md)  |  [DisplayName (нонемптистрингтипе)](displayname-nonemptystringtype.md)  |  [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="d8dae-111">[ImAddress (NonEmptyStringType)](imaddress-nonemptystringtype.md) | [DisplayName (NonEmptyStringType)](displayname-nonemptystringtype.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8dae-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d8dae-112">Parent elements</span></span>

<span data-ttu-id="d8dae-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d8dae-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d8dae-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="d8dae-114">Remarks</span></span>

<span data-ttu-id="d8dae-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8dae-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d8dae-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d8dae-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d8dae-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d8dae-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8dae-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d8dae-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d8dae-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d8dae-119">Schema name</span></span>  <br/> |<span data-ttu-id="d8dae-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d8dae-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d8dae-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d8dae-121">Validation file</span></span>  <br/> |<span data-ttu-id="d8dae-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d8dae-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8dae-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d8dae-123">Can be empty</span></span>  <br/> |<span data-ttu-id="d8dae-124">false</span><span class="sxs-lookup"><span data-stu-id="d8dae-124">false</span></span>  <br/> |
   

