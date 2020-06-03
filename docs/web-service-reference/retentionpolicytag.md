---
title: Retentionpolicytag используется
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f46679d0-9236-41e2-8624-72300079c67c
description: Элемент Retentionpolicytag используется указывает политику хранения для элемента почтового ящика.
ms.openlocfilehash: 3ece841e14e6cf11ab15e4a4d8b83a778ae32e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465179"
---
# <a name="retentionpolicytag"></a><span data-ttu-id="b9bd7-103">Retentionpolicytag используется</span><span class="sxs-lookup"><span data-stu-id="b9bd7-103">RetentionPolicyTag</span></span>

<span data-ttu-id="b9bd7-104">Элемент **retentionpolicytag используется** указывает политику хранения для элемента почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b9bd7-104">The **RetentionPolicyTag** element specifies the retention policy for a mailbox item.</span></span> 
  
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

 <span data-ttu-id="b9bd7-105">**ретентионполицитагтипе**</span><span class="sxs-lookup"><span data-stu-id="b9bd7-105">**RetentionPolicyTagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9bd7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b9bd7-106">Attributes and elements</span></span>

<span data-ttu-id="b9bd7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b9bd7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9bd7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b9bd7-108">Attributes</span></span>

<span data-ttu-id="b9bd7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9bd7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9bd7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b9bd7-110">Child elements</span></span>

<span data-ttu-id="b9bd7-111">[DisplayName (строка)](displayname-string.md)  |  [RetentionId](retentionid.md)  |  [Ретентионпериод](retentionperiod.md)  |  [Тип (елкфолдертипе)](type-elcfoldertype.md)  |  [RetentionAction](retentionaction.md)  |  [Description (описание](description.md)  |  ) [Отображается](isvisible.md)  |  [Оптединто](optedinto.md)  |  [Archive](isarchive.md)</span><span class="sxs-lookup"><span data-stu-id="b9bd7-111">[DisplayName (string)](displayname-string.md) | [RetentionId](retentionid.md) | [RetentionPeriod](retentionperiod.md) | [Type (ElcFolderType)](type-elcfoldertype.md) | [RetentionAction](retentionaction.md) | [Description](description.md) | [IsVisible](isvisible.md) | [OptedInto](optedinto.md) | [IsArchive](isarchive.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b9bd7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b9bd7-112">Parent elements</span></span>

[<span data-ttu-id="b9bd7-113">ретентионполицитагс</span><span class="sxs-lookup"><span data-stu-id="b9bd7-113">RetentionPolicyTags</span></span>](retentionpolicytags.md)
  
## <a name="remarks"></a><span data-ttu-id="b9bd7-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="b9bd7-114">Remarks</span></span>

<span data-ttu-id="b9bd7-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b9bd7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b9bd7-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b9bd7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9bd7-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b9bd7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9bd7-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b9bd7-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b9bd7-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b9bd7-119">Schema name</span></span>  <br/> |<span data-ttu-id="b9bd7-120">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b9bd7-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="b9bd7-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b9bd7-121">Validation file</span></span>  <br/> |<span data-ttu-id="b9bd7-122">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b9bd7-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b9bd7-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b9bd7-123">Can be empty</span></span>  <br/> ||
   

