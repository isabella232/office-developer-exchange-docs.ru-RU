---
title: GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 949871f7-0d10-498e-84aa-f0652f1193be
description: Элемент GetSearchableMailboxes содержит запрос на получение списка почтовых ящиков, у которых у клиента есть разрешение на выполнение поиска обнаружения электронных данных.
ms.openlocfilehash: a327f8766e53e9f1fae6928179d5a4b8e3d044a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530192"
---
# <a name="getsearchablemailboxes"></a><span data-ttu-id="d571f-103">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d571f-103">GetSearchableMailboxes</span></span>

<span data-ttu-id="d571f-104">Элемент **GetSearchableMailboxes** содержит запрос на получение списка почтовых ящиков, у которых у клиента есть разрешение на выполнение поиска обнаружения электронных данных.</span><span class="sxs-lookup"><span data-stu-id="d571f-104">The **GetSearchableMailboxes** element contains a request to get a list of mailboxes that the client has permission to perform an eDiscovery search.</span></span> 
  
```XML
<GetSearchableMailboxes>
   <SearchFilter/>
   <ExpandGroupMembership/>
</GetSearchableMailboxes>
```

 <span data-ttu-id="d571f-105">**жетсеарчаблемаилбоксестипе**</span><span class="sxs-lookup"><span data-stu-id="d571f-105">**GetSearchableMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d571f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d571f-106">Attributes and elements</span></span>

<span data-ttu-id="d571f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d571f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d571f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d571f-108">Attributes</span></span>

<span data-ttu-id="d571f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d571f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d571f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d571f-110">Child elements</span></span>

<span data-ttu-id="d571f-111">[SearchFilter](searchfilter.md)  |  [Експандграупмембершип](expandgroupmembership.md)</span><span class="sxs-lookup"><span data-stu-id="d571f-111">[SearchFilter](searchfilter.md) | [ExpandGroupMembership](expandgroupmembership.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d571f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d571f-112">Parent elements</span></span>

<span data-ttu-id="d571f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d571f-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d571f-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="d571f-114">Remarks</span></span>

<span data-ttu-id="d571f-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d571f-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d571f-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d571f-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d571f-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d571f-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d571f-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d571f-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d571f-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d571f-119">Schema name</span></span>  <br/> |<span data-ttu-id="d571f-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d571f-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d571f-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d571f-121">Validation file</span></span>  <br/> |<span data-ttu-id="d571f-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d571f-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d571f-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d571f-123">Can be empty</span></span>  <br/> ||
   

