---
title: RetentionPolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: Элемент RetentionPolicyTag указывает политику хранения для элементов почтового ящика.
ms.openlocfilehash: 2525f6d7a0ca583342d28dd9f4857a69b3a8c05a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835226"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="1e691-103">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="1e691-103">RetentionPolicyTag</span></span>

<span data-ttu-id="1e691-104">Элемент **RetentionPolicyTag** указывает политику хранения для элементов почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1e691-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
```XML
<RetentionPolicyTag>
   <DisplayName/>
   <RetentionId/>
   <RetentionPeriod/>
   <Type/>
   <RetentionAction/>
   <Description/>
   <IsVisible/>
   <OptedInto/>
   <IsArchive/>
</RetentionPolicyTag>
```

 <span data-ttu-id="1e691-105">**RetentionPolicyTagType**</span><span class="sxs-lookup"><span data-stu-id="1e691-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1e691-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1e691-106">Attributes and elements</span></span>

<span data-ttu-id="1e691-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1e691-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e691-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1e691-108">Attributes</span></span>

<span data-ttu-id="1e691-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1e691-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e691-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1e691-110">Child elements</span></span>

<span data-ttu-id="1e691-111">[Отображаемое имя (строка)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [типа (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Описание](description.md) | [IsVisible](isvisible.md)  |  [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="1e691-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e691-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1e691-112">Parent elements</span></span>

[<span data-ttu-id="1e691-113">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="1e691-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="1e691-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="1e691-114">Remarks</span></span>

<span data-ttu-id="1e691-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1e691-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1e691-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1e691-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e691-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1e691-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e691-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1e691-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e691-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1e691-119">Schema name</span></span>  <br/> |<span data-ttu-id="1e691-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1e691-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e691-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1e691-121">Validation file</span></span>  <br/> |<span data-ttu-id="1e691-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1e691-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e691-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1e691-123">Can be empty</span></span>  <br/> ||
   

