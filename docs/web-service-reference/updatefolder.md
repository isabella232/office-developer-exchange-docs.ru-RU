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
ms.openlocfilehash: 124ffd02a5ea2e7bf6f21cc7009dde08837906f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457048"
---
# <a name="updatefolder"></a><span data-ttu-id="72663-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="72663-103">UpdateFolder</span></span>

<span data-ttu-id="72663-104">Элемент **операцию UpdateFolder** представляет операцию, используемую для обновления свойств указанной папки.</span><span class="sxs-lookup"><span data-stu-id="72663-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="72663-105">**упдатефолдертипе**</span><span class="sxs-lookup"><span data-stu-id="72663-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72663-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="72663-106">Attributes and elements</span></span>

<span data-ttu-id="72663-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="72663-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72663-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="72663-108">Attributes</span></span>

<span data-ttu-id="72663-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72663-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72663-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="72663-110">Child elements</span></span>

|<span data-ttu-id="72663-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72663-111">**Element**</span></span>|<span data-ttu-id="72663-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72663-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72663-113">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="72663-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="72663-114">Содержит коллекцию изменений для указанной папки.</span><span class="sxs-lookup"><span data-stu-id="72663-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72663-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="72663-115">Parent elements</span></span>

<span data-ttu-id="72663-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="72663-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72663-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="72663-117">Remarks</span></span>

<span data-ttu-id="72663-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="72663-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72663-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="72663-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72663-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="72663-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72663-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="72663-121">Schema Name</span></span>  <br/> |<span data-ttu-id="72663-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="72663-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72663-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="72663-123">Validation File</span></span>  <br/> |<span data-ttu-id="72663-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="72663-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72663-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="72663-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="72663-126">False</span><span class="sxs-lookup"><span data-stu-id="72663-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72663-127">См. также</span><span class="sxs-lookup"><span data-stu-id="72663-127">See also</span></span>



[<span data-ttu-id="72663-128">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="72663-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

