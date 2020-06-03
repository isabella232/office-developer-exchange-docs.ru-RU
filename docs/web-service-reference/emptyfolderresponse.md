---
title: емптифолдерреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c900be49-3c90-41aa-aba5-bcf1116ec2aa
description: Элемент Емптифолдерреспонсе определяет ответ на запрос операции EmptyFolder.
ms.openlocfilehash: 9b20df8c0b095870185aab14dbd1f7ff4fc47def
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530679"
---
# <a name="emptyfolderresponse"></a><span data-ttu-id="c4dce-103">емптифолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="c4dce-103">EmptyFolderResponse</span></span>

<span data-ttu-id="c4dce-104">Элемент **емптифолдерреспонсе** определяет ответ на запрос [операции EmptyFolder](emptyfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c4dce-104">The **EmptyFolderResponse** element defines a response to an [EmptyFolder operation](emptyfolder-operation.md) request.</span></span> 
  
```XML
<EmptyFolderResponse>
   <ResponseMessages/>
</EmptyFolderResponse>
```

 <span data-ttu-id="c4dce-105">**емптифолдерреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="c4dce-105">**EmptyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4dce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c4dce-106">Attributes and elements</span></span>

<span data-ttu-id="c4dce-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c4dce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4dce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c4dce-108">Attributes</span></span>

<span data-ttu-id="c4dce-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c4dce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4dce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c4dce-110">Child elements</span></span>

|<span data-ttu-id="c4dce-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c4dce-111">**Element**</span></span>|<span data-ttu-id="c4dce-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c4dce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4dce-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="c4dce-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c4dce-114">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4dce-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4dce-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c4dce-115">Parent elements</span></span>

<span data-ttu-id="c4dce-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="c4dce-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c4dce-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="c4dce-117">Remarks</span></span>

<span data-ttu-id="c4dce-118">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4dce-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4dce-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c4dce-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4dce-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c4dce-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c4dce-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c4dce-121">Schema name</span></span>  <br/> |<span data-ttu-id="c4dce-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="c4dce-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c4dce-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c4dce-123">Validation file</span></span>  <br/> |<span data-ttu-id="c4dce-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="c4dce-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4dce-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c4dce-125">Can be empty</span></span>  <br/> |<span data-ttu-id="c4dce-126">False</span><span class="sxs-lookup"><span data-stu-id="c4dce-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4dce-127">См. также</span><span class="sxs-lookup"><span data-stu-id="c4dce-127">See also</span></span>



[<span data-ttu-id="c4dce-128">Операция EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="c4dce-128">EmptyFolder operation</span></span>](emptyfolder-operation.md)
  
[<span data-ttu-id="c4dce-129">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="c4dce-129">EmptyFolder</span></span>](emptyfolder.md)


- [<span data-ttu-id="c4dce-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c4dce-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

