---
title: InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc2ca69e-eea7-4334-b046-ec0b04d8f8c6
description: Элемент InstallApp указывает запрос на установку приложения.
ms.openlocfilehash: 003a72507813677484b2d6ee75f8ff577df169e3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468007"
---
# <a name="installapp"></a><span data-ttu-id="57564-103">InstallApp</span><span class="sxs-lookup"><span data-stu-id="57564-103">InstallApp</span></span>

<span data-ttu-id="57564-104">Элемент **InstallAPP** указывает запрос на установку приложения.</span><span class="sxs-lookup"><span data-stu-id="57564-104">The **InstallApp** element specifies the request to install an app.</span></span> 
  
```XML
<InstallApp>
    <Manifest/>
</InstallApp>
```

 <span data-ttu-id="57564-105">**инсталлапптипе**</span><span class="sxs-lookup"><span data-stu-id="57564-105">**InstallAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57564-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57564-106">Attributes and elements</span></span>

<span data-ttu-id="57564-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="57564-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57564-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57564-108">Attributes</span></span>

<span data-ttu-id="57564-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="57564-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57564-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57564-110">Child elements</span></span>

|<span data-ttu-id="57564-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57564-111">**Element**</span></span>|<span data-ttu-id="57564-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57564-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57564-113">Манифест</span><span class="sxs-lookup"><span data-stu-id="57564-113">Manifest</span></span>](manifest.md) <br/> |<span data-ttu-id="57564-114">Содержит файл манифеста приложения в кодировке Base64.</span><span class="sxs-lookup"><span data-stu-id="57564-114">Contains the base64-encoded app manifest file.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57564-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57564-115">Parent elements</span></span>

<span data-ttu-id="57564-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="57564-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57564-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="57564-117">Remarks</span></span>

<span data-ttu-id="57564-118">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="57564-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="57564-119">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="57564-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57564-120">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57564-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57564-121">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57564-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57564-122">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57564-122">Schema Name</span></span>  <br/> |<span data-ttu-id="57564-123">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="57564-123">Message schema</span></span>  <br/> |
|<span data-ttu-id="57564-124">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57564-124">Validation File</span></span>  <br/> |<span data-ttu-id="57564-125">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="57564-125">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57564-126">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57564-126">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="57564-127">См. также</span><span class="sxs-lookup"><span data-stu-id="57564-127">See also</span></span>



- [<span data-ttu-id="57564-128">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="57564-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

