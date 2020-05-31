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
description: Элемент операцию UpdateFolder представляет операцию, используемую для обновления свойств указанной папки.
ms.openlocfilehash: 9a86bf6b3b5917600b3b09f23b3ee4e9cdc0364f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840325"
---
# <a name="updatefolder"></a><span data-ttu-id="3b292-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="3b292-103">UpdateFolder</span></span>

<span data-ttu-id="3b292-104">Элемент **операцию UpdateFolder** представляет операцию, используемую для обновления свойств указанной папки.</span><span class="sxs-lookup"><span data-stu-id="3b292-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="3b292-105">**упдатефолдертипе**</span><span class="sxs-lookup"><span data-stu-id="3b292-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b292-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b292-106">Attributes and elements</span></span>

<span data-ttu-id="3b292-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3b292-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b292-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b292-108">Attributes</span></span>

<span data-ttu-id="3b292-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b292-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b292-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b292-110">Child elements</span></span>

|<span data-ttu-id="3b292-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b292-111">**Element**</span></span>|<span data-ttu-id="3b292-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b292-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b292-113">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="3b292-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="3b292-114">Содержит коллекцию изменений для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="3b292-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b292-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b292-115">Parent elements</span></span>

<span data-ttu-id="3b292-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b292-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b292-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b292-117">Remarks</span></span>

<span data-ttu-id="3b292-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3b292-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b292-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b292-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b292-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b292-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b292-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b292-121">Schema Name</span></span>  <br/> |<span data-ttu-id="3b292-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="3b292-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b292-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b292-123">Validation File</span></span>  <br/> |<span data-ttu-id="3b292-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3b292-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b292-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b292-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b292-126">False</span><span class="sxs-lookup"><span data-stu-id="3b292-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b292-127">См. также</span><span class="sxs-lookup"><span data-stu-id="3b292-127">See also</span></span>



[<span data-ttu-id="3b292-128">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="3b292-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

