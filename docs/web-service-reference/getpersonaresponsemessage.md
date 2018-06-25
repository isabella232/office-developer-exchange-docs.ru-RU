---
title: GetPersonaResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a5bf44c6-c46b-442d-98d4-8b49fdf14b30
description: GetPersonaResponseMessage содержит ответ данные, получаемые из GetPersona запроса.
ms.openlocfilehash: 7d38daac9c7c3a74ba9d9670c2bd16dcf2cd47e3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762891"
---
# <a name="getpersonaresponsemessage"></a><span data-ttu-id="338f1-103">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="338f1-103">GetPersonaResponseMessage</span></span>

<span data-ttu-id="338f1-104">**GetPersonaResponseMessage** содержит ответ данные, получаемые из **GetPersona** запроса.</span><span class="sxs-lookup"><span data-stu-id="338f1-104">The **GetPersonaResponseMessage** contains the response data resulting from a **GetPersona** request.</span></span> 
  
```XML
<GetPersonaResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Persona/>
</GetPersonaResponseMessage>
```

 <span data-ttu-id="338f1-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="338f1-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="338f1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="338f1-106">Attributes and elements</span></span>

<span data-ttu-id="338f1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="338f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="338f1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="338f1-108">Attributes</span></span>

<span data-ttu-id="338f1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="338f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="338f1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="338f1-110">Child elements</span></span>

<span data-ttu-id="338f1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [пользователя](persona.md)</span><span class="sxs-lookup"><span data-stu-id="338f1-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Persona](persona.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="338f1-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="338f1-112">Parent elements</span></span>

[<span data-ttu-id="338f1-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="338f1-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="338f1-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="338f1-114">Remarks</span></span>

<span data-ttu-id="338f1-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="338f1-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="338f1-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="338f1-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="338f1-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="338f1-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="338f1-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="338f1-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="338f1-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="338f1-119">Schema name</span></span>  <br/> |<span data-ttu-id="338f1-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="338f1-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="338f1-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="338f1-121">Validation file</span></span>  <br/> |<span data-ttu-id="338f1-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="338f1-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="338f1-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="338f1-123">Can be empty</span></span>  <br/> ||
   

