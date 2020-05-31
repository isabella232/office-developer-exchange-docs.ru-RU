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
ms.openlocfilehash: db73cb7f1922d845c9565753ff8d4917b82b1259
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833701"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a><span data-ttu-id="66f23-103">жетусерретентионполицитагсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="66f23-103">GetUserRetentionPolicyTagsResponseMessage</span></span>

<span data-ttu-id="66f23-104">Элемент **жетусерретентионполицитагсреспонсемессаже** указывает ответное сообщение для запроса **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="66f23-104">The **GetUserRetentionPolicyTagsResponseMessage** element specifies the response message for a **GetUserRetentionPolicyTags** request.</span></span> 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 <span data-ttu-id="66f23-105">**жетусерретентионполицитагсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="66f23-105">**GetUserRetentionPolicyTagsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="66f23-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="66f23-106">Attributes and elements</span></span>

<span data-ttu-id="66f23-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="66f23-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66f23-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="66f23-108">Attributes</span></span>

<span data-ttu-id="66f23-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="66f23-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66f23-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="66f23-110">Child elements</span></span>

<span data-ttu-id="66f23-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [RetentionPolicyTags](retentionpolicytags.md) [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md)дескриптивелинккэй мессажексмл ретентионполицитагс |  | </span><span class="sxs-lookup"><span data-stu-id="66f23-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [RetentionPolicyTags](retentionpolicytags.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66f23-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="66f23-112">Parent elements</span></span>

[<span data-ttu-id="66f23-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="66f23-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="66f23-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="66f23-114">Remarks</span></span>

<span data-ttu-id="66f23-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="66f23-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="66f23-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="66f23-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="66f23-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="66f23-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="66f23-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="66f23-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="66f23-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="66f23-119">Schema name</span></span>  <br/> |<span data-ttu-id="66f23-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="66f23-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="66f23-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="66f23-121">Validation file</span></span>  <br/> |<span data-ttu-id="66f23-122">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="66f23-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="66f23-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="66f23-123">Can be empty</span></span>  <br/> |<span data-ttu-id="66f23-124">false</span><span class="sxs-lookup"><span data-stu-id="66f23-124">false</span></span>  <br/> |
   

