---
title: шаредфолдерид
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
description: Элемент Шаредфолдерид представляет идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом операции GetSharingFolder.
ms.openlocfilehash: 546e148540708725bcf335f39bf69d193124d210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466124"
---
# <a name="sharedfolderid"></a><span data-ttu-id="c2639-103">шаредфолдерид</span><span class="sxs-lookup"><span data-stu-id="c2639-103">SharedFolderId</span></span>

<span data-ttu-id="c2639-104">Элемент **шаредфолдерид** представляет идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c2639-104">The **SharedFolderId** element represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<SharedFolderId/>
```

 <span data-ttu-id="c2639-105">**нонемптистрингтипе**</span><span class="sxs-lookup"><span data-stu-id="c2639-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2639-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c2639-106">Attributes and elements</span></span>

<span data-ttu-id="c2639-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c2639-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2639-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c2639-108">Attributes</span></span>

<span data-ttu-id="c2639-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2639-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2639-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c2639-110">Child elements</span></span>

<span data-ttu-id="c2639-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2639-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2639-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c2639-112">Parent elements</span></span>

|<span data-ttu-id="c2639-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2639-113">**Element**</span></span>|<span data-ttu-id="c2639-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2639-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2639-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="c2639-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="c2639-116">Определяет запрос на получение идентификатора локальной папки указанной общей папки.</span><span class="sxs-lookup"><span data-stu-id="c2639-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c2639-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c2639-117">Text value</span></span>

<span data-ttu-id="c2639-118">Текстовое значение — это строка, представляющая идентификатор общей папки, идентификатор локальной папки, который должен быть возвращен запросом [операции GetSharingFolder](getsharingfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c2639-118">The text value is a string that represents the identifier of the shared folder the local folder identifier for which should be returned by a [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c2639-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="c2639-119">Remarks</span></span>

<span data-ttu-id="c2639-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2639-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2639-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c2639-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2639-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c2639-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2639-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c2639-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c2639-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c2639-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2639-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c2639-125">Validation File</span></span>  <br/> |<span data-ttu-id="c2639-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c2639-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2639-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c2639-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2639-128">False</span><span class="sxs-lookup"><span data-stu-id="c2639-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2639-129">См. также</span><span class="sxs-lookup"><span data-stu-id="c2639-129">See also</span></span>



[<span data-ttu-id="c2639-130">Операция GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="c2639-130">GetSharingFolder operation</span></span>](getsharingfolder-operation.md)


- [<span data-ttu-id="c2639-131">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c2639-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

