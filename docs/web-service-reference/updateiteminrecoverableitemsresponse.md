---
title: упдатеитеминрековераблеитемсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2f61b038-eba0-40fc-8af2-c3db5cc5a420
description: Элемент Упдатеитеминрековераблеитемсреспонсе указывает ответ на запрос Упдатеитеминрековераблеитемс.
ms.openlocfilehash: 2cb9bcb2752599a546c1391d6ea306735b3b0c78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840354"
---
# <a name="updateiteminrecoverableitemsresponse"></a><span data-ttu-id="28459-103">упдатеитеминрековераблеитемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="28459-103">UpdateItemInRecoverableItemsResponse</span></span>

<span data-ttu-id="28459-104">Элемент **упдатеитеминрековераблеитемсреспонсе** указывает ответ на запрос **упдатеитеминрековераблеитемс** .</span><span class="sxs-lookup"><span data-stu-id="28459-104">The **UpdateItemInRecoverableItemsResponse** element specifies the response to an **UpdateItemInRecoverableItems** request.</span></span> 
  
```XML
<UpdateItemInRecoverableItemsResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <Attachments/>
   <ConflictResults/>
</UpdateItemInRecoverableItemsResponse>
```

 <span data-ttu-id="28459-105">**упдатеитеминрековераблеитемсреспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="28459-105">**UpdateItemInRecoverableItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28459-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="28459-106">Attributes and elements</span></span>

<span data-ttu-id="28459-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="28459-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28459-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="28459-108">Attributes</span></span>

<span data-ttu-id="28459-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="28459-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28459-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="28459-110">Child elements</span></span>

<span data-ttu-id="28459-111">[Мессажетекст](messagetext.md) | [респонсекоде](responsecode.md) | [MessageXml](messagexml.md)[Attachments](attachments-ex15websvcsotherref.md)[DescriptiveLinkKey](descriptivelinkkey.md) | [ConflictResults](conflictresults.md) [Items](items.md)дескриптивелинккэй мессажексмл | элементы | вложения конфликтресултс | </span><span class="sxs-lookup"><span data-stu-id="28459-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [Items](items.md) | [Attachments](attachments-ex15websvcsotherref.md) | [ConflictResults](conflictresults.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="28459-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="28459-112">Parent elements</span></span>

<span data-ttu-id="28459-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="28459-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28459-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="28459-114">Remarks</span></span>

<span data-ttu-id="28459-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="28459-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="28459-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="28459-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28459-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="28459-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28459-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="28459-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28459-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="28459-119">Schema name</span></span>  <br/> |<span data-ttu-id="28459-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="28459-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28459-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="28459-121">Validation file</span></span>  <br/> |<span data-ttu-id="28459-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="28459-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28459-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="28459-123">Can be empty</span></span>  <br/> |<span data-ttu-id="28459-124">false</span><span class="sxs-lookup"><span data-stu-id="28459-124">false</span></span>  <br/> |
   

