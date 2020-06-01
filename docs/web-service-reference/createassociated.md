---
title: креатеассоЦиатед
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAssociated
api_type:
- schema
ms.assetid: 742a6136-6015-4924-bae4-f3868127e966
description: Элемент КреатеассоЦиатед указывает, может ли клиент создать связанную таблицу содержимого. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e88d7670fd9ef848221dab8cc145395bcb11e5bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460794"
---
# <a name="createassociated"></a><span data-ttu-id="cce06-104">креатеассоЦиатед</span><span class="sxs-lookup"><span data-stu-id="cce06-104">CreateAssociated</span></span>

<span data-ttu-id="cce06-105">Элемент **креатеассоЦиатед** указывает, может ли клиент создать связанную таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="cce06-105">The **CreateAssociated** element indicates whether a client can create an associated contents table.</span></span> <span data-ttu-id="cce06-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cce06-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<CreateAssociated>true or false</CreateAssociated>
```

 <span data-ttu-id="cce06-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="cce06-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cce06-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cce06-108">Attributes and elements</span></span>

<span data-ttu-id="cce06-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cce06-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cce06-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cce06-110">Attributes</span></span>

<span data-ttu-id="cce06-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cce06-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cce06-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cce06-112">Child elements</span></span>

<span data-ttu-id="cce06-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cce06-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cce06-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cce06-114">Parent elements</span></span>

|<span data-ttu-id="cce06-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cce06-115">**Element**</span></span>|<span data-ttu-id="cce06-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cce06-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cce06-117">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="cce06-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="cce06-118">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="cce06-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="cce06-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cce06-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cce06-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cce06-120">Text value</span></span>

<span data-ttu-id="cce06-121">Текстовое значение **true** указывает, что клиент может создать связанную таблицу содержимого.</span><span class="sxs-lookup"><span data-stu-id="cce06-121">A text value of **true** indicates that a client can create an associated contents table.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cce06-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="cce06-122">Remarks</span></span>

<span data-ttu-id="cce06-123">Это свойство используется только для объектов Folder.</span><span class="sxs-lookup"><span data-stu-id="cce06-123">This property is only used on folder objects.</span></span>
  
<span data-ttu-id="cce06-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cce06-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cce06-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cce06-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cce06-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cce06-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cce06-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cce06-127">Schema Name</span></span>  <br/> |<span data-ttu-id="cce06-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cce06-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="cce06-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cce06-129">Validation File</span></span>  <br/> |<span data-ttu-id="cce06-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cce06-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cce06-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cce06-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="cce06-132">False</span><span class="sxs-lookup"><span data-stu-id="cce06-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cce06-133">См. также</span><span class="sxs-lookup"><span data-stu-id="cce06-133">See also</span></span>



- [<span data-ttu-id="cce06-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cce06-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="cce06-135">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="cce06-135">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

