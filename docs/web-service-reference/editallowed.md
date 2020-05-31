---
title: едиталловед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: Элемент Едиталловед указывает, можно ли изменять управление правами на доступ к данным.
ms.openlocfilehash: 48c7d751c018bf5702b05b41eeaa7ad350189e3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762250"
---
# <a name="editallowed"></a><span data-ttu-id="a7ed9-103">едиталловед</span><span class="sxs-lookup"><span data-stu-id="a7ed9-103">EditAllowed</span></span>

<span data-ttu-id="a7ed9-104">Элемент **едиталловед** указывает, можно ли изменять управление правами на доступ к данным.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="a7ed9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a7ed9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7ed9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a7ed9-106">Attributes and elements</span></span>

<span data-ttu-id="a7ed9-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7ed9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a7ed9-108">Attributes</span></span>

<span data-ttu-id="a7ed9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7ed9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a7ed9-110">Child elements</span></span>

<span data-ttu-id="a7ed9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7ed9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a7ed9-112">Parent elements</span></span>

|<span data-ttu-id="a7ed9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a7ed9-113">**Element**</span></span>|<span data-ttu-id="a7ed9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a7ed9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7ed9-115">ригхтсманажементлиценседата</span><span class="sxs-lookup"><span data-stu-id="a7ed9-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="a7ed9-116">Указывает сведения о лицензии на управление правами.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7ed9-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a7ed9-117">Text value</span></span>

<span data-ttu-id="a7ed9-118">Текстовое значение **true** для элемента **едиталловед** указывает на то, что Управление правами на доступ к данным (IRM) можно изменить.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="a7ed9-119">Значение **false** указывает, что Управление правами на доступ к данным не может быть изменено.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a7ed9-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="a7ed9-120">Remarks</span></span>

<span data-ttu-id="a7ed9-121">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a7ed9-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7ed9-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7ed9-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a7ed9-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7ed9-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a7ed9-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7ed9-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a7ed9-125">Schema Name</span></span>  <br/> |<span data-ttu-id="a7ed9-126">Схема типа</span><span class="sxs-lookup"><span data-stu-id="a7ed9-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="a7ed9-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a7ed9-127">Validation File</span></span>  <br/> |<span data-ttu-id="a7ed9-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a7ed9-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7ed9-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a7ed9-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a7ed9-130">См. также</span><span class="sxs-lookup"><span data-stu-id="a7ed9-130">See also</span></span>



- [<span data-ttu-id="a7ed9-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7ed9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

