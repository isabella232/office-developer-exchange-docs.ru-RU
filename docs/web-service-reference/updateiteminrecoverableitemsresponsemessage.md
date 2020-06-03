---
title: упдатеитеминрековераблеитемсреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 96259756-322e-4c24-ac76-0cd9c32e0d6d
description: Элемент Упдатеитеминрековераблеитемсреспонсемессаже указывает ответ на запрос Упдатеитеминрековераблеитемс.
ms.openlocfilehash: 021631f5c30eebbf4d7ae0aad35a85b99a23925f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466537"
---
# <a name="updateiteminrecoverableitemsresponsemessage"></a><span data-ttu-id="3609e-103">упдатеитеминрековераблеитемсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="3609e-103">UpdateItemInRecoverableItemsResponseMessage</span></span>

<span data-ttu-id="3609e-104">Элемент **упдатеитеминрековераблеитемсреспонсемессаже** указывает ответ на запрос **упдатеитеминрековераблеитемс** .</span><span class="sxs-lookup"><span data-stu-id="3609e-104">The **UpdateItemInRecoverableItemsResponseMessage** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKet/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponseMessage>
```

 <span data-ttu-id="3609e-105">**упдатеитеминрековераблеитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="3609e-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3609e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3609e-106">Attributes and elements</span></span>

<span data-ttu-id="3609e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3609e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3609e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3609e-108">Attributes</span></span>

<span data-ttu-id="3609e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3609e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3609e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3609e-110">Child elements</span></span>

<span data-ttu-id="3609e-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Элементы](items.md)  |  [Вложения](attachments-ex15websvcsotherref.md)  |  [Конфликтресултс](conflictresults.md)</span><span class="sxs-lookup"><span data-stu-id="3609e-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3609e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3609e-112">Parent elements</span></span>

<span data-ttu-id="3609e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3609e-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3609e-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="3609e-114">Remarks</span></span>

<span data-ttu-id="3609e-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3609e-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3609e-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3609e-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3609e-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3609e-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3609e-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3609e-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/message  <br/> |
|<span data-ttu-id="3609e-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3609e-119">Schema name</span></span>  <br/> |<span data-ttu-id="3609e-120">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="3609e-120">Message schema</span></span>  <br/> |
|<span data-ttu-id="3609e-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3609e-121">Validation file</span></span>  <br/> |<span data-ttu-id="3609e-122">Message. xsd</span><span class="sxs-lookup"><span data-stu-id="3609e-122">Message.xsd</span></span>  <br/> |
|<span data-ttu-id="3609e-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3609e-123">Can be empty</span></span>  <br/> |<span data-ttu-id="3609e-124">false</span><span class="sxs-lookup"><span data-stu-id="3609e-124">false</span></span>  <br/> |
   

