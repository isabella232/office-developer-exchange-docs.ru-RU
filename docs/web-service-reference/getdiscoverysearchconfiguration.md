---
title: GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e15dbfca-3b9d-463e-94ec-4f1b6115bee3
description: Элемент GetDiscoverySearchConfiguration указывает запрос на получение конфигурации поиска для обнаружения электронных данных.
ms.openlocfilehash: 821c5e1429c160e326f6d99df3ff4fcc831b83d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461004"
---
# <a name="getdiscoverysearchconfiguration"></a><span data-ttu-id="518f1-103">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="518f1-103">GetDiscoverySearchConfiguration</span></span>

<span data-ttu-id="518f1-104">Элемент **GetDiscoverySearchConfiguration** указывает запрос на получение конфигурации поиска для обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="518f1-104">The **GetDiscoverySearchConfiguration** element specifies a request to retrieve the eDiscovery search configuration.</span></span> 
  
```XML
<GetDiscoverySearchConfiguration>
    <SearchId/>
    <ExpandGroupMembership/>
</GetDiscoverySearchConfiguration>
```

 <span data-ttu-id="518f1-105">**жетдисковерисеарчконфигуратионтипе**</span><span class="sxs-lookup"><span data-stu-id="518f1-105">**GetDiscoverySearchConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="518f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="518f1-106">Attributes and elements</span></span>

<span data-ttu-id="518f1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="518f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="518f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="518f1-108">Attributes</span></span>

<span data-ttu-id="518f1-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="518f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="518f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="518f1-110">Child elements</span></span>

|<span data-ttu-id="518f1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="518f1-111">**Element**</span></span>|<span data-ttu-id="518f1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="518f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="518f1-113">сеарчид</span><span class="sxs-lookup"><span data-stu-id="518f1-113">SearchId</span></span>](searchid.md) <br/> |<span data-ttu-id="518f1-114">Задает идентификатор поиска.</span><span class="sxs-lookup"><span data-stu-id="518f1-114">Specifies the identifier of the search.</span></span>  <br/> |
|[<span data-ttu-id="518f1-115">експандграупмембершип</span><span class="sxs-lookup"><span data-stu-id="518f1-115">ExpandGroupMembership</span></span>](expandgroupmembership.md) <br/> |<span data-ttu-id="518f1-116">Содержит логическое значение, указывающее, следует ли расширять членство в группе, возвращенной из запроса **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="518f1-116">Contains a Boolean value that indicates whether to expand the membership of the group returned from a **GetSearchableMailboxes** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="518f1-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="518f1-117">Parent elements</span></span>

<span data-ttu-id="518f1-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="518f1-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="518f1-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="518f1-119">Remarks</span></span>

<span data-ttu-id="518f1-120">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="518f1-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="518f1-121">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="518f1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="518f1-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="518f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="518f1-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="518f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="518f1-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="518f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="518f1-125">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="518f1-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="518f1-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="518f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="518f1-127">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="518f1-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="518f1-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="518f1-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="518f1-129">См. также</span><span class="sxs-lookup"><span data-stu-id="518f1-129">See also</span></span>



- [<span data-ttu-id="518f1-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="518f1-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

