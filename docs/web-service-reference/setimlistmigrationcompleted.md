---
title: SetImListMigrationCompleted
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4b806441-0429-44c4-90b7-1ae5c6ab9128
description: Элемент SetImListMigrationCompleted представляет запрос для указания того, содержит ли мгновенного обмена сообщениями элементов, используемых в клиентов системы обмена сообщениями в хранилище Exchange.
ms.openlocfilehash: 602583594aa171d49a1af2b70664301bf8ff1244
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835431"
---
# <a name="setimlistmigrationcompleted"></a><span data-ttu-id="5b605-103">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="5b605-103">SetImListMigrationCompleted</span></span>

<span data-ttu-id="5b605-104">Элемент **SetImListMigrationCompleted** представляет запрос для указания того, содержит ли мгновенного обмена сообщениями элементов, используемых в клиентов системы обмена сообщениями в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b605-104">The **SetImListMigrationCompleted** element represents a request to indicate whether the Exchange store contains the instant messaging items used by instant messaging clients.</span></span> 
  
```XML
<SetImListMigrationCompleted>
   <ImListMigrationCompleted/>
</SetImListMigrationCompleted>
```

 <span data-ttu-id="5b605-105">**SetImListMigrationCompletedType**</span><span class="sxs-lookup"><span data-stu-id="5b605-105">**SetImListMigrationCompletedType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b605-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5b605-106">Attributes and elements</span></span>

<span data-ttu-id="5b605-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5b605-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b605-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5b605-108">Attributes</span></span>

<span data-ttu-id="5b605-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b605-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b605-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5b605-110">Child elements</span></span>

[<span data-ttu-id="5b605-111">ImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="5b605-111">ImListMigrationCompleted</span></span>](imlistmigrationcompleted.md)
  
### <a name="parent-elements"></a><span data-ttu-id="5b605-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5b605-112">Parent elements</span></span>

<span data-ttu-id="5b605-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5b605-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5b605-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="5b605-114">Remarks</span></span>

<span data-ttu-id="5b605-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5b605-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5b605-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b605-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b605-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5b605-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b605-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5b605-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b605-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5b605-119">Schema name</span></span>  <br/> |<span data-ttu-id="5b605-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="5b605-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b605-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5b605-121">Validation file</span></span>  <br/> |<span data-ttu-id="5b605-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5b605-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b605-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5b605-123">Can be empty</span></span>  <br/> |<span data-ttu-id="5b605-124">Нет</span><span class="sxs-lookup"><span data-stu-id="5b605-124">false</span></span>  <br/> |
   

