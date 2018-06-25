---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: Элемент SharedFolderId представляет идентификатор общей папки, идентификатор локальной папки, для которого возвращаются при запрос операции GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835477"
---
# <a name="sharedfolderid"></a><span data-ttu-id="ff42c-103">SharedFolderId</span><span class="sxs-lookup"><span data-stu-id="ff42c-103">SharedFolderId</span></span>

<span data-ttu-id="ff42c-104">Элемент **SharedFolderId** представляет идентификатор общей папки, идентификатор локальной папки, для которого возвращаются при [GetSharingFolder операция](getsharingfolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="ff42c-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="ff42c-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="ff42c-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff42c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ff42c-106">Attributes and elements</span></span>

<span data-ttu-id="ff42c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ff42c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff42c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ff42c-108">Attributes</span></span>

<span data-ttu-id="ff42c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff42c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff42c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ff42c-110">Child elements</span></span>

<span data-ttu-id="ff42c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff42c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff42c-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ff42c-112">Parent elements</span></span>

|<span data-ttu-id="ff42c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ff42c-113">**Element**</span></span>|<span data-ttu-id="ff42c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ff42c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff42c-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ff42c-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="ff42c-116">Определяет запрос на получение идентификатора локальной папки указанной общей папке.</span><span class="sxs-lookup"><span data-stu-id="ff42c-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff42c-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ff42c-117">Text value</span></span>

<span data-ttu-id="ff42c-118">Текстовое значение — это строка, которая представляет идентификатор элемента общей папке идентификатор локальной папки, для которого возвращаются при [GetSharingFolder операции](getsharingfolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="ff42c-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ff42c-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="ff42c-119">Remarks</span></span>

<span data-ttu-id="ff42c-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff42c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff42c-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ff42c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff42c-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ff42c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff42c-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ff42c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ff42c-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ff42c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff42c-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ff42c-125">Validation File</span></span>  <br/> |<span data-ttu-id="ff42c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ff42c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff42c-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ff42c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff42c-128">False</span><span class="sxs-lookup"><span data-stu-id="ff42c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff42c-129">См. также</span><span class="sxs-lookup"><span data-stu-id="ff42c-129">See also</span></span>



[<span data-ttu-id="ff42c-130">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ff42c-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="ff42c-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ff42c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

