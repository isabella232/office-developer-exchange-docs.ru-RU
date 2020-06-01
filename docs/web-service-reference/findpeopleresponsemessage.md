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
ms.openlocfilehash: 5a2ce7b8643fff9d4a93b62459638d3a99605c98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466376"
---
# <a name="findpeopleresponsemessage"></a><span data-ttu-id="f71af-103">финдпеоплереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f71af-103">FindPeopleResponseMessage</span></span>

<span data-ttu-id="f71af-104">Элемент **финдпеоплереспонсемессаже** указывает ответное сообщение для запроса **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="f71af-104">The **FindPeopleResponseMessage** element specifies the response message for a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="f71af-105">**финдпеоплереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="f71af-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f71af-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f71af-106">Attributes and elements</span></span>

<span data-ttu-id="f71af-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f71af-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f71af-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f71af-108">Attributes</span></span>

<span data-ttu-id="f71af-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f71af-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f71af-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f71af-110">Child elements</span></span>

<span data-ttu-id="f71af-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Люди](people.md)  |  [Тоталнумберофпеоплеинвиев](totalnumberofpeopleinview.md)</span><span class="sxs-lookup"><span data-stu-id="f71af-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [People](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f71af-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f71af-112">Parent elements</span></span>

[<span data-ttu-id="f71af-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="f71af-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="f71af-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="f71af-114">Remarks</span></span>

<span data-ttu-id="f71af-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f71af-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f71af-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f71af-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f71af-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f71af-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f71af-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f71af-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f71af-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f71af-119">Schema name</span></span>  <br/> |<span data-ttu-id="f71af-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f71af-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f71af-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f71af-121">Validation file</span></span>  <br/> |<span data-ttu-id="f71af-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f71af-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f71af-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f71af-123">Can be empty</span></span>  <br/> |<span data-ttu-id="f71af-124">false</span><span class="sxs-lookup"><span data-stu-id="f71af-124">false</span></span>  <br/> |
   

