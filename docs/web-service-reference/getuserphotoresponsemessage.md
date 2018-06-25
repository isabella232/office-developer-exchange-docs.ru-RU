---
title: GetUserPhotoResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54d43fe6-9f7b-4f84-920a-bd686c65b059
description: Элемент GetUserPhotoResponseMessage содержит ответ на запрос GetUserPhoto.
ms.openlocfilehash: fa817b59527f616afed84d8548e3a18e6c971e2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833696"
---
# <a name="getuserphotoresponsemessage"></a><span data-ttu-id="33ca7-103">GetUserPhotoResponseMessage</span><span class="sxs-lookup"><span data-stu-id="33ca7-103">GetUserPhotoResponseMessage</span></span>

<span data-ttu-id="33ca7-104">Элемент **GetUserPhotoResponseMessage** содержит ответ на запрос GetUserPhoto.</span><span class="sxs-lookup"><span data-stu-id="33ca7-104">The **GetUserPhotoResponseMessage** element contains the response to a GetUserPhoto request.</span></span> 
  
```XML
<GetUserPhotoResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <HasChanged/>
   <PictureData/>
</GetUserPhotoResponseMessage>
```

 <span data-ttu-id="33ca7-105">**GetUserPhotoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="33ca7-105">**GetUserPhotoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33ca7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33ca7-106">Attributes and elements</span></span>

<span data-ttu-id="33ca7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="33ca7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33ca7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33ca7-108">Attributes</span></span>

<span data-ttu-id="33ca7-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="33ca7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33ca7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33ca7-110">Child elements</span></span>

<span data-ttu-id="33ca7-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [Свойства](picturedata.md)</span><span class="sxs-lookup"><span data-stu-id="33ca7-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [HasChanged](haschanged.md) | [PictureData](picturedata.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33ca7-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33ca7-112">Parent elements</span></span>

[<span data-ttu-id="33ca7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="33ca7-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="33ca7-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="33ca7-114">Remarks</span></span>

<span data-ttu-id="33ca7-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="33ca7-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="33ca7-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="33ca7-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33ca7-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33ca7-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33ca7-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33ca7-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="33ca7-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33ca7-119">Schema name</span></span>  <br/> |<span data-ttu-id="33ca7-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="33ca7-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="33ca7-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33ca7-121">Validation file</span></span>  <br/> |<span data-ttu-id="33ca7-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="33ca7-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="33ca7-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33ca7-123">Can be empty</span></span>  <br/> ||
   

