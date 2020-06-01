---
title: исманажедфолдерсрут
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
description: Элемент Исманажедфолдерсрут указывает, является ли управляемая папка корневой для всех управляемых папок.
ms.openlocfilehash: 4373dba9dce92de8e175948d889f0806e100fa6c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466026"
---
# <a name="ismanagedfoldersroot"></a><span data-ttu-id="8704b-103">исманажедфолдерсрут</span><span class="sxs-lookup"><span data-stu-id="8704b-103">IsManagedFoldersRoot</span></span>

<span data-ttu-id="8704b-104">Элемент **исманажедфолдерсрут** указывает, является ли управляемая папка корневой для всех управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="8704b-104">The **IsManagedFoldersRoot** element indicates whether the managed folder is the root for all managed folders.</span></span> 
  
```xml
<IsManagedFoldersRoot/>
```

 <span data-ttu-id="8704b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="8704b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8704b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8704b-106">Attributes and elements</span></span>

<span data-ttu-id="8704b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8704b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8704b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8704b-108">Attributes</span></span>

<span data-ttu-id="8704b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8704b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8704b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8704b-110">Child elements</span></span>

<span data-ttu-id="8704b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8704b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8704b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8704b-112">Parent elements</span></span>

|<span data-ttu-id="8704b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8704b-113">**Element**</span></span>|<span data-ttu-id="8704b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8704b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8704b-115">манажедфолдеринформатион</span><span class="sxs-lookup"><span data-stu-id="8704b-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="8704b-116">Содержит сведения об управляемой папке.</span><span class="sxs-lookup"><span data-stu-id="8704b-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8704b-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8704b-117">Text value</span></span>

<span data-ttu-id="8704b-118">При наличии этого элемента необходимо указать текстовое значение, представляющее логическое значение.</span><span class="sxs-lookup"><span data-stu-id="8704b-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="8704b-119">Значение **true** указывает, что папка является корневой папкой управляемой папки; значение **false** указывает, что папка не является корневой папкой управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="8704b-119">A value of **true** indicates that the folder is the root folder of the managed folder; a value of **false** indicates that the folder is not the root folder of the managed folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8704b-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="8704b-120">Remarks</span></span>

<span data-ttu-id="8704b-121">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8704b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8704b-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8704b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8704b-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8704b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8704b-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8704b-124">Schema name</span></span>  <br/> |<span data-ttu-id="8704b-125">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8704b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8704b-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8704b-126">Validation file</span></span>  <br/> |<span data-ttu-id="8704b-127">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8704b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8704b-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8704b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="8704b-129">False</span><span class="sxs-lookup"><span data-stu-id="8704b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8704b-130">См. также</span><span class="sxs-lookup"><span data-stu-id="8704b-130">See also</span></span>



- [<span data-ttu-id="8704b-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8704b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

