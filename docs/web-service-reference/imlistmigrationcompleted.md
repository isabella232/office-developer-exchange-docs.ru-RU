---
title: ImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6eed9502-5d9e-4345-ba23-3582ff487147
description: Элемент ImListMigrationCompleted указывает, содержит ли хранилище Exchange мгновенного обмена сообщениями элементов, используемых в клиентов системы обмена сообщениями.
ms.openlocfilehash: 25f1b583b354a71958fbc8052c492726dc0eb7db
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833893"
---
# <a name="imlistmigrationcompleted"></a><span data-ttu-id="d2a52-103">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="d2a52-103">ImListMigrationCompleted</span></span>

<span data-ttu-id="d2a52-104">Элемент **ImListMigrationCompleted** указывает, содержит ли хранилище Exchange обмена мгновенными сообщениями элементов, используемых в клиентов системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="d2a52-104">The **ImListMigrationCompleted** element indicates whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<ImListMigrationCompleted>true | false</ImListMigrationCompleted>
```

 <span data-ttu-id="d2a52-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d2a52-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2a52-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d2a52-106">Attributes and elements</span></span>

<span data-ttu-id="d2a52-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d2a52-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2a52-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d2a52-108">Attributes</span></span>

<span data-ttu-id="d2a52-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d2a52-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2a52-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d2a52-110">Child elements</span></span>

<span data-ttu-id="d2a52-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d2a52-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2a52-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d2a52-112">Parent elements</span></span>

[<span data-ttu-id="d2a52-113">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="d2a52-113">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted.md)
  
## <a name="text-value"></a><span data-ttu-id="d2a52-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d2a52-114">Text value</span></span>

<span data-ttu-id="d2a52-115">Текстовое значение **true** для элемента **ImListMigrationCompleted** указывает, что хранить обмена мгновенными сообщениями, хранения перенесен в Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2a52-115">A text value of **true** for the **ImListMigrationCompleted** element indicates that the instant messaging contacts store has been migrated to the Exchange store.</span></span> <span data-ttu-id="d2a52-116">Значение **false** указывает, что хранилище контактов мгновенного сообщения не были перенесены.</span><span class="sxs-lookup"><span data-stu-id="d2a52-116">A value of **false** indicates that the instant message contacts store has not been migrated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d2a52-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="d2a52-117">Remarks</span></span>

<span data-ttu-id="d2a52-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d2a52-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2a52-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d2a52-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2a52-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d2a52-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2a52-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d2a52-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2a52-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d2a52-122">Schema name</span></span>  <br/> |<span data-ttu-id="d2a52-123">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d2a52-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2a52-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d2a52-124">Validation file</span></span>  <br/> |<span data-ttu-id="d2a52-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2a52-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2a52-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d2a52-126">Can be empty</span></span>  <br/> ||
   

