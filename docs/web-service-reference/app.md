---
title: Приложение
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 92b776b5-fec6-4443-a606-51ccb06f7afd
description: Элемент App содержит сведения о XML-файле манифеста для почтового приложения, установленного в почтовом ящике.
ms.openlocfilehash: c63bbbf6eb3bf718b2cf81e67d9ec978b3bc5f8d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761388"
---
# <a name="app"></a><span data-ttu-id="46715-103">Приложение</span><span class="sxs-lookup"><span data-stu-id="46715-103">App</span></span>

<span data-ttu-id="46715-104">Элемент **app** содержит сведения о XML-файле манифеста для почтового приложения, установленного в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="46715-104">The **App** element contains information about an XML manifest file for a mail app that is installed in a mailbox.</span></span> 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="46715-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="46715-105">Attributes and elements</span></span>

<span data-ttu-id="46715-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="46715-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="46715-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="46715-107">Attributes</span></span>

<span data-ttu-id="46715-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="46715-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="46715-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="46715-109">Child elements</span></span>

<span data-ttu-id="46715-110">[Metadata](metadata-ex15websvcsotherref.md) | [Манифест](manifest.md) метаданных</span><span class="sxs-lookup"><span data-stu-id="46715-110">[Metadata](metadata-ex15websvcsotherref.md) | [Manifest](manifest.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="46715-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="46715-111">Parent elements</span></span>

[<span data-ttu-id="46715-112">Приложения</span><span class="sxs-lookup"><span data-stu-id="46715-112">Apps</span></span>](apps.md)
  
## <a name="remarks"></a><span data-ttu-id="46715-113">Примечания</span><span class="sxs-lookup"><span data-stu-id="46715-113">Remarks</span></span>

<span data-ttu-id="46715-114">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="46715-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="46715-115">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="46715-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="46715-116">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="46715-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="46715-117">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="46715-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="46715-118">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="46715-118">Schema Name</span></span>  <br/> |<span data-ttu-id="46715-119">Схема Types</span><span class="sxs-lookup"><span data-stu-id="46715-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="46715-120">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="46715-120">Validation File</span></span>  <br/> |<span data-ttu-id="46715-121">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="46715-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="46715-122">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="46715-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="46715-123">False</span><span class="sxs-lookup"><span data-stu-id="46715-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="46715-124">См. также</span><span class="sxs-lookup"><span data-stu-id="46715-124">See also</span></span>

- [<span data-ttu-id="46715-125">Приложения</span><span class="sxs-lookup"><span data-stu-id="46715-125">Apps</span></span>](apps.md)
- [<span data-ttu-id="46715-126">Метаданные</span><span class="sxs-lookup"><span data-stu-id="46715-126">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="46715-127">Манифест</span><span class="sxs-lookup"><span data-stu-id="46715-127">Manifest</span></span>](manifest.md)
- [<span data-ttu-id="46715-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="46715-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

