---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: Элемент Request GetImItems определяет запрос на получение сведений об указанных группах мгновенных сообщений и контактных лиц обмена мгновенными сообщениями.
ms.openlocfilehash: e3973cbbf800ffe91472b9c733c4d4a927b91c9f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456453"
---
# <a name="getimitems"></a><span data-ttu-id="f8fa0-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="f8fa0-103">GetImItems</span></span>

<span data-ttu-id="f8fa0-104">Элемент Request **GetImItems** определяет запрос на получение сведений об указанных группах мгновенных сообщений и контактных лиц обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="f8fa0-105">**жетимитемстипе**</span><span class="sxs-lookup"><span data-stu-id="f8fa0-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8fa0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f8fa0-106">Attributes and elements</span></span>

<span data-ttu-id="f8fa0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8fa0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f8fa0-108">Attributes</span></span>

<span data-ttu-id="f8fa0-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8fa0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f8fa0-110">Child elements</span></span>

<span data-ttu-id="f8fa0-111">[Контактидс](contactids.md)  |  [Граупидс](groupids.md)  |  [Екстендедпропертиес (нонемптяррайофекстендедфиелдурис)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="f8fa0-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f8fa0-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f8fa0-112">Parent elements</span></span>

<span data-ttu-id="f8fa0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f8fa0-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="f8fa0-114">Remarks</span></span>

<span data-ttu-id="f8fa0-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f8fa0-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8fa0-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8fa0-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f8fa0-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8fa0-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f8fa0-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8fa0-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f8fa0-119">Schema name</span></span>  <br/> |<span data-ttu-id="f8fa0-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f8fa0-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8fa0-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f8fa0-121">Validation file</span></span>  <br/> |<span data-ttu-id="f8fa0-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f8fa0-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8fa0-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f8fa0-123">Can be empty</span></span>  <br/> ||
   

