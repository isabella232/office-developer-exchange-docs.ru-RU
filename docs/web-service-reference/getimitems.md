---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: Элемент запроса GetImItems определяет запрос на получение сведений о указанными группами мгновенного обмена сообщениями и обмена мгновенными сообщениями контакта пользователей.
ms.openlocfilehash: ff7d520dde44fac6e9278633c1ad46b07b38d6c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762813"
---
# <a name="getimitems"></a><span data-ttu-id="70e9b-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="70e9b-103">GetImItems</span></span>

<span data-ttu-id="70e9b-104">Элемент запроса **GetImItems** определяет запрос на получение сведений о указанными группами мгновенного обмена сообщениями и обмена мгновенными сообщениями контакта пользователей.</span><span class="sxs-lookup"><span data-stu-id="70e9b-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="70e9b-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="70e9b-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70e9b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="70e9b-106">Attributes and elements</span></span>

<span data-ttu-id="70e9b-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="70e9b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70e9b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="70e9b-108">Attributes</span></span>

<span data-ttu-id="70e9b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e9b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70e9b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="70e9b-110">Child elements</span></span>

<span data-ttu-id="70e9b-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="70e9b-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70e9b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="70e9b-112">Parent elements</span></span>

<span data-ttu-id="70e9b-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="70e9b-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70e9b-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="70e9b-114">Remarks</span></span>

<span data-ttu-id="70e9b-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="70e9b-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="70e9b-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="70e9b-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70e9b-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="70e9b-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70e9b-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="70e9b-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70e9b-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="70e9b-119">Schema name</span></span>  <br/> |<span data-ttu-id="70e9b-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="70e9b-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70e9b-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="70e9b-121">Validation file</span></span>  <br/> |<span data-ttu-id="70e9b-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="70e9b-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70e9b-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="70e9b-123">Can be empty</span></span>  <br/> ||
   

