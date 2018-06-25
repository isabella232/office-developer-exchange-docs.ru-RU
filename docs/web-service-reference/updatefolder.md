---
title: UpdateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 412d0683-2819-40c5-a0ae-f613499a7b66
description: Элемент UpdateFolder представляет операцию, которая используется для обновления свойств для указанной папки.
ms.openlocfilehash: 9a86bf6b3b5917600b3b09f23b3ee4e9cdc0364f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840325"
---
# <a name="updatefolder"></a><span data-ttu-id="9a8bf-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9a8bf-103">UpdateFolder</span></span>

<span data-ttu-id="9a8bf-104">Элемент **UpdateFolder** представляет операцию, которая используется для обновления свойств для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="9a8bf-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="9a8bf-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a8bf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9a8bf-106">Attributes and elements</span></span>

<span data-ttu-id="9a8bf-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a8bf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9a8bf-108">Attributes</span></span>

<span data-ttu-id="9a8bf-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a8bf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9a8bf-110">Child elements</span></span>

|<span data-ttu-id="9a8bf-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9a8bf-111">**Element**</span></span>|<span data-ttu-id="9a8bf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9a8bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a8bf-113">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="9a8bf-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="9a8bf-114">Содержит коллекцию изменений для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9a8bf-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9a8bf-115">Parent elements</span></span>

<span data-ttu-id="9a8bf-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a8bf-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="9a8bf-117">Remarks</span></span>

<span data-ttu-id="9a8bf-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9a8bf-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a8bf-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9a8bf-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a8bf-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9a8bf-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a8bf-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9a8bf-121">Schema Name</span></span>  <br/> |<span data-ttu-id="9a8bf-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="9a8bf-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a8bf-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9a8bf-123">Validation File</span></span>  <br/> |<span data-ttu-id="9a8bf-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9a8bf-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a8bf-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9a8bf-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a8bf-126">False</span><span class="sxs-lookup"><span data-stu-id="9a8bf-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a8bf-127">См. также</span><span class="sxs-lookup"><span data-stu-id="9a8bf-127">See also</span></span>



[<span data-ttu-id="9a8bf-128">Операцию UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="9a8bf-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

