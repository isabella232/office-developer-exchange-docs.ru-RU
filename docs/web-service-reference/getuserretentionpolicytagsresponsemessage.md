---
title: жетусерретентионполицитагсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: Элемент Жетусерретентионполицитагсреспонсемессаже указывает ответное сообщение для запроса GetUserRetentionPolicyTags.
ms.openlocfilehash: e65266e72010f42a2052bbb8cfab21ea4059f92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461809"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="c2920-103">жетусерретентионполицитагсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="c2920-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="c2920-104">Элемент **жетусерретентионполицитагсреспонсемессаже** указывает ответное сообщение для запроса **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="c2920-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="c2920-105">**жетусерретентионполицитагсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="c2920-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2920-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c2920-106">Attributes and elements</span></span>

<span data-ttu-id="c2920-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c2920-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2920-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c2920-108">Attributes</span></span>

<span data-ttu-id="c2920-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c2920-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2920-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c2920-110">Child elements</span></span>

<span data-ttu-id="c2920-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Ретентионполицитагс](retentionpolicytags.md)</span><span class="sxs-lookup"><span data-stu-id="c2920-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c2920-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c2920-112">Parent elements</span></span>

[<span data-ttu-id="c2920-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c2920-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="c2920-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="c2920-114">Remarks</span></span>

<span data-ttu-id="c2920-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c2920-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c2920-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2920-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2920-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c2920-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2920-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c2920-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2920-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c2920-119">Schema name</span></span>  <br/> |<span data-ttu-id="c2920-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c2920-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2920-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c2920-121">Validation file</span></span>  <br/> |<span data-ttu-id="c2920-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c2920-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2920-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c2920-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c2920-124">false</span><span class="sxs-lookup"><span data-stu-id="c2920-124">false</span></span>  <br/> |
   

