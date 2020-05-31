---
title: ретентионполицитипе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: abce5b3e-971d-42fc-aeea-caa7202214de
description: Элемент Ретентионполицитипе указывает тип политики хранения, применяемый к элементам в беседе.
ms.openlocfilehash: dacb3fa75611cbd6e6e29eab7c791dfd8964c9ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835229"
---
# <a name="retentionpolicytype"></a><span data-ttu-id="b54a8-103">ретентионполицитипе</span><span class="sxs-lookup"><span data-stu-id="b54a8-103">RetentionPolicyType</span></span>

<span data-ttu-id="b54a8-104">Элемент **ретентионполицитипе** указывает тип политики хранения, применяемый к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="b54a8-104">The **RetentionPolicyType** element specifies the retention policy type applied to items in a conversation.</span></span> 
  
```XML
<RetentionPolicyType> Delete | Archive </RetentionPolicyType>
```

 <span data-ttu-id="b54a8-105">**RetentionType**</span><span class="sxs-lookup"><span data-stu-id="b54a8-105">**RetentionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b54a8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b54a8-106">Attributes and elements</span></span>

<span data-ttu-id="b54a8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b54a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b54a8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b54a8-108">Attributes</span></span>

<span data-ttu-id="b54a8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b54a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b54a8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b54a8-110">Child elements</span></span>

<span data-ttu-id="b54a8-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="b54a8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b54a8-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b54a8-112">Parent elements</span></span>

[<span data-ttu-id="b54a8-113">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="b54a8-113">ConversationAction</span></span>](conversationaction.md)
  
## <a name="text-value"></a><span data-ttu-id="b54a8-114">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b54a8-114">Text value</span></span>

<span data-ttu-id="b54a8-115">Текстовое значение элемента **ретентионполицитипе** — это тип хранения, применяемый к элементам в беседе.</span><span class="sxs-lookup"><span data-stu-id="b54a8-115">The text value of the **RetentionPolicyType** element is the retention type applied to items in a conversation.</span></span> <span data-ttu-id="b54a8-116">Текстовое значение **Delete** указывает на то, что элементы беседы удаляются по истечении срока хранения.</span><span class="sxs-lookup"><span data-stu-id="b54a8-116">The text value of **Delete** indicates that the items in the conversation are deleted when the retention hold expires.</span></span> <span data-ttu-id="b54a8-117">Текстовое значение **архива** указывает на то, что элементы беседы перемещаются в архивный почтовый ящик при истечении срока хранения.</span><span class="sxs-lookup"><span data-stu-id="b54a8-117">The text value of **Archive** indicates that the items in the conversation are moved to the archive mailbox when the retention hold expires.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b54a8-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="b54a8-118">Remarks</span></span>

<span data-ttu-id="b54a8-119">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b54a8-119">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b54a8-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b54a8-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b54a8-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b54a8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b54a8-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b54a8-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b54a8-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b54a8-123">Schema name</span></span>  <br/> |<span data-ttu-id="b54a8-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b54a8-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="b54a8-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b54a8-125">Validation file</span></span>  <br/> |<span data-ttu-id="b54a8-126">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b54a8-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b54a8-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b54a8-127">Can be empty</span></span>  <br/> ||
   

