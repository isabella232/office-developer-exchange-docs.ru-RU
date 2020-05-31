---
title: финдпеоплереспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba686738-e654-404d-ab54-83c71d030350
description: Элемент Финдпеоплереспонсемессаже указывает ответное сообщение для запроса FindPeople.
ms.openlocfilehash: 205f20b26b5097d24de45c5a5f9681f3557a6f87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762597"
---
# <a name="findpeopleresponsemessage"></a><span data-ttu-id="f3106-103">финдпеоплереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f3106-103">FindPeopleResponseMessage</span></span>

<span data-ttu-id="f3106-104">Элемент **финдпеоплереспонсемессаже** указывает ответное сообщение для запроса **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="f3106-104">The **FindPeopleResponseMessage** element specifies the response message for a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <People/>
   <TotalNumberOfPeopleInView/>
</FindPeopleResponseMessage>
```

 <span data-ttu-id="f3106-105">**финдпеоплереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f3106-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3106-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3106-106">Attributes and elements</span></span>

<span data-ttu-id="f3106-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f3106-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3106-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3106-108">Attributes</span></span>

<span data-ttu-id="f3106-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3106-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3106-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3106-110">Child elements</span></span>

<span data-ttu-id="f3106-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [MessageXml](messagexml.md)[DescriptiveLinkKey](descriptivelinkkey.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md) дескриптивелинккэй мессажексмл | [люди](people.md)тоталнумберофпеоплеинвиев | </span><span class="sxs-lookup"><span data-stu-id="f3106-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [People](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3106-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3106-112">Parent elements</span></span>

[<span data-ttu-id="f3106-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f3106-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="f3106-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="f3106-114">Remarks</span></span>

<span data-ttu-id="f3106-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3106-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3106-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3106-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3106-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3106-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3106-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3106-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3106-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3106-119">Schema name</span></span>  <br/> |<span data-ttu-id="f3106-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3106-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3106-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3106-121">Validation file</span></span>  <br/> |<span data-ttu-id="f3106-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f3106-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3106-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3106-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f3106-124">false</span><span class="sxs-lookup"><span data-stu-id="f3106-124">false</span></span>  <br/> |
   

