---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: Элемент ImListMigrationCompleted указывает, содержит ли хранилище Exchange элементы для обмена мгновенными сообщениями, используемые клиентами обмена мгновенными сообщениями.
ms.openlocfilehash: 09f37d6e3663aab7cb98fc922f727ddd604f2acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456026"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="4486b-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="4486b-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="4486b-104">Элемент **ImListMigrationCompleted** указывает, содержит ли хранилище Exchange элементы для обмена мгновенными сообщениями, используемые клиентами обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="4486b-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="4486b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4486b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4486b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4486b-106">Attributes and elements</span></span>

<span data-ttu-id="4486b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4486b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4486b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4486b-108">Attributes</span></span>

<span data-ttu-id="4486b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4486b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4486b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4486b-110">Child elements</span></span>

<span data-ttu-id="4486b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4486b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4486b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4486b-112">Parent elements</span></span>

[<span data-ttu-id="4486b-113">сетимлистмигратионкомплетед</span><span class="sxs-lookup"><span data-stu-id="4486b-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="4486b-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4486b-114">Text value</span></span>

<span data-ttu-id="4486b-115">Текстовое значение **true** для элемента **ImListMigrationCompleted** указывает на то, что хранилище контактов для обмена мгновенными сообщениями было перенесено в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4486b-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="4486b-116">Значение **false** указывает, что хранилище контактов для обмена мгновенными сообщениями не было перенесено.</span><span class="sxs-lookup"><span data-stu-id="4486b-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4486b-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="4486b-117">Remarks</span></span>

<span data-ttu-id="4486b-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4486b-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4486b-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4486b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4486b-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4486b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4486b-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4486b-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4486b-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4486b-122">Schema name</span></span>  <br/> |<span data-ttu-id="4486b-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4486b-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4486b-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4486b-124">Validation file</span></span>  <br/> |<span data-ttu-id="4486b-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4486b-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4486b-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4486b-126">Can be empty</span></span>  <br/> ||
   

