---
title: Чтение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Read
api_type:
- schema
ms.assetid: b14637e9-1695-4b7e-b078-ae527c2e4303
description: Элемент Read указывает, может ли клиент прочитать папку или элемент. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: d75285e0ab14c4f53d73cb7f4349196e07c3c521
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468315"
---
# <a name="read"></a><span data-ttu-id="725fd-104">Чтение</span><span class="sxs-lookup"><span data-stu-id="725fd-104">Read</span></span>

<span data-ttu-id="725fd-105">Элемент **Read** указывает, может ли клиент прочитать папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="725fd-105">The **Read** element indicates whether a client can read a folder or item.</span></span> <span data-ttu-id="725fd-106">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="725fd-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<Read>true or false</Read>
```

 <span data-ttu-id="725fd-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="725fd-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="725fd-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="725fd-108">Attributes and elements</span></span>

<span data-ttu-id="725fd-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="725fd-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="725fd-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="725fd-110">Attributes</span></span>

<span data-ttu-id="725fd-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="725fd-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="725fd-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="725fd-112">Child elements</span></span>

<span data-ttu-id="725fd-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="725fd-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="725fd-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="725fd-114">Parent elements</span></span>

|<span data-ttu-id="725fd-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="725fd-115">**Element**</span></span>|<span data-ttu-id="725fd-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="725fd-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="725fd-117">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="725fd-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="725fd-118">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="725fd-118">Contains the rights of the client based on the permission settings for the item or folder.</span></span> <span data-ttu-id="725fd-119">Этот элемент появился в Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="725fd-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="725fd-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="725fd-120">Text value</span></span>

<span data-ttu-id="725fd-121">Текстовое значение **true** указывает, что клиент может читать элементы папки.</span><span class="sxs-lookup"><span data-stu-id="725fd-121">A text value of **true** indicates that a client can read an item of folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="725fd-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="725fd-122">Remarks</span></span>

<span data-ttu-id="725fd-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="725fd-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="725fd-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="725fd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="725fd-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="725fd-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="725fd-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="725fd-126">Schema Name</span></span>  <br/> |<span data-ttu-id="725fd-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="725fd-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="725fd-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="725fd-128">Validation File</span></span>  <br/> |<span data-ttu-id="725fd-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="725fd-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="725fd-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="725fd-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="725fd-131">False</span><span class="sxs-lookup"><span data-stu-id="725fd-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="725fd-132">См. также</span><span class="sxs-lookup"><span data-stu-id="725fd-132">See also</span></span>



- [<span data-ttu-id="725fd-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="725fd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="725fd-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="725fd-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

