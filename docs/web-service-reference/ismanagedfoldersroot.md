---
title: IsManagedFoldersRoot
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsManagedFoldersRoot
api_type:
- schema
ms.assetid: 00823fb9-bf8b-49bb-8e1b-d698c6d4063f
description: Элемент IsManagedFoldersRoot указывает, является ли управляемых папок корневого каталога для всех управляемых папок.
ms.openlocfilehash: 3484a3fef56545a9a8d56af65f56f75205918ec7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834044"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="bd34e-103">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="bd34e-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="bd34e-104">Элемент **IsManagedFoldersRoot** указывает, является ли управляемых папок корневого каталога для всех управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="bd34e-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="bd34e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="bd34e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd34e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd34e-106">Attributes and elements</span></span>

<span data-ttu-id="bd34e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bd34e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd34e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd34e-108">Attributes</span></span>

<span data-ttu-id="bd34e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd34e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd34e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd34e-110">Child elements</span></span>

<span data-ttu-id="bd34e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd34e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bd34e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd34e-112">Parent elements</span></span>

|<span data-ttu-id="bd34e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd34e-113">**Element**</span></span>|<span data-ttu-id="bd34e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd34e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd34e-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="bd34e-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="bd34e-116">Содержит сведения об управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="bd34e-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bd34e-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bd34e-117">Text value</span></span>

<span data-ttu-id="bd34e-118">Текстовое значение, представляющее логическое значение является обязательным, если присутствует этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bd34e-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="bd34e-119">Значение **true** указывает, что папка является корневой папке управляемой папки; значение **false** указывает, что папка не находится в корневой папке управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="bd34e-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bd34e-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="bd34e-120">Remarks</span></span>

<span data-ttu-id="bd34e-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bd34e-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd34e-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd34e-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd34e-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd34e-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd34e-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd34e-124">Schema name</span></span>  <br/> |<span data-ttu-id="bd34e-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bd34e-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd34e-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd34e-126">Validation file</span></span>  <br/> |<span data-ttu-id="bd34e-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bd34e-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd34e-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd34e-128">Can be empty</span></span>  <br/> |<span data-ttu-id="bd34e-129">False</span><span class="sxs-lookup"><span data-stu-id="bd34e-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd34e-130">См. также</span><span class="sxs-lookup"><span data-stu-id="bd34e-130">See also</span></span>



- [<span data-ttu-id="bd34e-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd34e-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

