---
title: ContactId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86f66275-1e39-48ed-bd89-ac3bffc465a7
description: Элемент ContactId однозначно идентифицирует контакт.
ms.openlocfilehash: 17e8012283078d5d6e2cd1d2e88eef37b008be42
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463183"
---
# <a name="contactid"></a><span data-ttu-id="0b479-103">ContactId</span><span class="sxs-lookup"><span data-stu-id="0b479-103">ContactId</span></span>

<span data-ttu-id="0b479-104">Элемент **ContactId** однозначно идентифицирует контакт.</span><span class="sxs-lookup"><span data-stu-id="0b479-104">The **ContactId** element uniquely identifies a contact.</span></span> 
  
```XML
<ContactId Id="" ChangeKey=""/>
```

 <span data-ttu-id="0b479-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="0b479-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b479-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b479-106">Attributes and elements</span></span>

<span data-ttu-id="0b479-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0b479-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b479-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b479-108">Attributes</span></span>

|<span data-ttu-id="0b479-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0b479-109">**Attribute**</span></span>|<span data-ttu-id="0b479-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b479-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0b479-111">Id</span><span class="sxs-lookup"><span data-stu-id="0b479-111">Id</span></span>  <br/> |<span data-ttu-id="0b479-112">Текстовое значение атрибута **ID** — идентификатор элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="0b479-112">The text value of the **Id** attribute is the identifier of the contact item.</span></span>  <br/> |
|<span data-ttu-id="0b479-113">чанжекэй</span><span class="sxs-lookup"><span data-stu-id="0b479-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="0b479-114">Текстовое значение атрибута **чанжекэй** — это ключ изменения элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="0b479-114">The text value of the **ChangeKey** attribute is the change key of the contact item.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0b479-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b479-115">Child elements</span></span>

<span data-ttu-id="0b479-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0b479-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0b479-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b479-117">Parent elements</span></span>

<span data-ttu-id="0b479-118">[AddImContactToGroup](addimcontacttogroup.md)  |  [RemoveContactFromImList](removecontactfromimlist.md)  |  [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span><span class="sxs-lookup"><span data-stu-id="0b479-118">[AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0b479-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="0b479-119">Remarks</span></span>

<span data-ttu-id="0b479-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0b479-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0b479-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0b479-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b479-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0b479-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b479-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0b479-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b479-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0b479-124">Schema name</span></span>  <br/> |<span data-ttu-id="0b479-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0b479-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b479-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0b479-126">Validation file</span></span>  <br/> |<span data-ttu-id="0b479-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0b479-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b479-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0b479-128">Can be empty</span></span>  <br/> |<span data-ttu-id="0b479-129">false</span><span class="sxs-lookup"><span data-stu-id="0b479-129">false</span></span>  <br/> |
   

