---
title: GetAppManifestsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 86cf88f4-09c4-436a-a100-ac5cba0c4388
description: Элемент GetAppManifestsResponse определяет ответа на запрос GetAppManifests операции.
ms.openlocfilehash: ae9d1d853023a5b42db2e8fee2ed57f585433f69
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354150"
---
# <a name="getappmanifestsresponse"></a><span data-ttu-id="1715f-103">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="1715f-103">GetAppManifestsResponse</span></span>

<span data-ttu-id="1715f-104">Элемент **GetAppManifestsResponse** определяет ответа на запрос **GetAppManifests** операции.</span><span class="sxs-lookup"><span data-stu-id="1715f-104">The **GetAppManifestsResponse** element defines the response for a **GetAppManifests** operation request.</span></span> 
  
```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Manifests/>
</GetAppManifestsResponse>
```

```xml
<GetAppManifestsResponse>
    <ResponseCode/>
    <Apps/>
</GetAppManifestsResponse>
```

<span data-ttu-id="1715f-105">**GetAppManifestsResponseType**</span><span class="sxs-lookup"><span data-stu-id="1715f-105">**GetAppManifestsResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1715f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1715f-106">Attributes and elements</span></span>

<span data-ttu-id="1715f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1715f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1715f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1715f-108">Attributes</span></span>

<span data-ttu-id="1715f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1715f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1715f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1715f-110">Child elements</span></span>

<span data-ttu-id="1715f-111">[ResponseCode](responsecode.md) | [манифестов](manifests.md) | [приложений](apps.md)</span><span class="sxs-lookup"><span data-stu-id="1715f-111">[ResponseCode](responsecode.md) | [Manifests](manifests.md) | [Apps](apps.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1715f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1715f-112">Parent elements</span></span>

<span data-ttu-id="1715f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="1715f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1715f-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="1715f-114">Remarks</span></span>

<span data-ttu-id="1715f-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1715f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1715f-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1715f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1715f-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1715f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1715f-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1715f-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1715f-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1715f-119">Schema Name</span></span>  <br/> |<span data-ttu-id="1715f-120">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="1715f-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="1715f-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1715f-121">Validation File</span></span>  <br/> |<span data-ttu-id="1715f-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1715f-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1715f-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1715f-123">Can Be Empty</span></span>  <br/> |<span data-ttu-id="1715f-124">False</span><span class="sxs-lookup"><span data-stu-id="1715f-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1715f-125">См. также</span><span class="sxs-lookup"><span data-stu-id="1715f-125">See also</span></span>

- [<span data-ttu-id="1715f-126">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1715f-126">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

