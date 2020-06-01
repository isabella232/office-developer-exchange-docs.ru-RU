---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: Элемент RefreshSharingFolder определяет запрос на обновление указанной локальной папки. Это базовый элемент для операции RefreshSharingFolder.
ms.openlocfilehash: 4454607fa2c3114cc7279fd7c30f8aee74707baa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467930"
---
# <a name="refreshsharingfolder"></a><span data-ttu-id="dc528-104">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="dc528-104">RefreshSharingFolder</span></span>

<span data-ttu-id="dc528-105">Элемент **RefreshSharingFolder** определяет запрос на обновление указанной локальной папки.</span><span class="sxs-lookup"><span data-stu-id="dc528-105">The **RefreshSharingFolder** element defines a request to refresh the specified local folder.</span></span> <span data-ttu-id="dc528-106">Это базовый элемент для [операции RefreshSharingFolder](refreshsharingfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="dc528-106">It is the base element for the [RefreshSharingFolder operation](refreshsharingfolder-operation.md).</span></span>
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 <span data-ttu-id="dc528-107">**рефрешшарингфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="dc528-107">**RefreshSharingFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dc528-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dc528-108">Attributes and elements</span></span>

<span data-ttu-id="dc528-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dc528-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc528-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dc528-110">Attributes</span></span>

<span data-ttu-id="dc528-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="dc528-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc528-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dc528-112">Child elements</span></span>

|<span data-ttu-id="dc528-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dc528-113">**Element**</span></span>|<span data-ttu-id="dc528-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dc528-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc528-115">шарингфолдерид</span><span class="sxs-lookup"><span data-stu-id="dc528-115">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="dc528-116">Представляет идентификатор локальной папки в отношении совместного доступа.</span><span class="sxs-lookup"><span data-stu-id="dc528-116">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc528-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dc528-117">Parent elements</span></span>

<span data-ttu-id="dc528-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="dc528-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dc528-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="dc528-119">Remarks</span></span>

<span data-ttu-id="dc528-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dc528-120">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc528-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dc528-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc528-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dc528-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dc528-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dc528-123">Schema Name</span></span>  <br/> |<span data-ttu-id="dc528-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dc528-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dc528-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dc528-125">Validation File</span></span>  <br/> |<span data-ttu-id="dc528-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dc528-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dc528-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dc528-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="dc528-128">False</span><span class="sxs-lookup"><span data-stu-id="dc528-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc528-129">См. также</span><span class="sxs-lookup"><span data-stu-id="dc528-129">See also</span></span>



- [<span data-ttu-id="dc528-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dc528-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

