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
ms.openlocfilehash: b5870164b059d2e50930ee33c09cbd030501f171
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460360"
---
# <a name="app"></a><span data-ttu-id="b2596-103">Приложение</span><span class="sxs-lookup"><span data-stu-id="b2596-103">App</span></span>

<span data-ttu-id="b2596-104">Элемент **app** содержит сведения о XML-файле манифеста для почтового приложения, установленного в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b2596-104">The **App** element contains information about an XML manifest file for a mail app that is installed in a mailbox.</span></span> 
  
```XML
<App>
    <Metadata/>
    <Manifest/>
</App>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b2596-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b2596-105">Attributes and elements</span></span>

<span data-ttu-id="b2596-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b2596-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b2596-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b2596-107">Attributes</span></span>

<span data-ttu-id="b2596-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b2596-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b2596-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b2596-109">Child elements</span></span>

<span data-ttu-id="b2596-110">[Metadata (метаданные](metadata-ex15websvcsotherref.md)  |  ) [Manifest](manifest.md)</span><span class="sxs-lookup"><span data-stu-id="b2596-110">[Metadata](metadata-ex15websvcsotherref.md) | [Manifest](manifest.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b2596-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b2596-111">Parent elements</span></span>

[<span data-ttu-id="b2596-112">Приложения</span><span class="sxs-lookup"><span data-stu-id="b2596-112">Apps</span></span>](apps.md)
  
## <a name="remarks"></a><span data-ttu-id="b2596-113">Примечания</span><span class="sxs-lookup"><span data-stu-id="b2596-113">Remarks</span></span>

<span data-ttu-id="b2596-114">Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="b2596-114">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="b2596-115">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b2596-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b2596-116">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b2596-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b2596-117">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b2596-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b2596-118">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b2596-118">Schema Name</span></span>  <br/> |<span data-ttu-id="b2596-119">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b2596-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="b2596-120">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b2596-120">Validation File</span></span>  <br/> |<span data-ttu-id="b2596-121">Неприменимо</span><span class="sxs-lookup"><span data-stu-id="b2596-121">Not applicable</span></span>  <br/> |
|<span data-ttu-id="b2596-122">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b2596-122">Can be Empty</span></span>  <br/> |<span data-ttu-id="b2596-123">False</span><span class="sxs-lookup"><span data-stu-id="b2596-123">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b2596-124">См. также</span><span class="sxs-lookup"><span data-stu-id="b2596-124">See also</span></span>

- [<span data-ttu-id="b2596-125">Приложения</span><span class="sxs-lookup"><span data-stu-id="b2596-125">Apps</span></span>](apps.md)
- [<span data-ttu-id="b2596-126">Метаданные</span><span class="sxs-lookup"><span data-stu-id="b2596-126">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="b2596-127">Манифест</span><span class="sxs-lookup"><span data-stu-id="b2596-127">Manifest</span></span>](manifest.md)
- [<span data-ttu-id="b2596-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b2596-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

