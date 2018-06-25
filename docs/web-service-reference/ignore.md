---
title: Пропуск
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ignore
api_type:
- schema
ms.assetid: 7789eec5-ceec-43f2-84d5-d0d15b734076
description: Элемент игнорировать определяет элементы, чтобы пропустить во время синхронизации.
ms.openlocfilehash: 0ecff9bfeb1257552b7e52c0115e9e814edecd4b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833858"
---
# <a name="ignore"></a><span data-ttu-id="7e5a2-103">Пропуск</span><span class="sxs-lookup"><span data-stu-id="7e5a2-103">Ignore</span></span>

<span data-ttu-id="7e5a2-104">Элемент **Игнорировать** определяет элементы, чтобы пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="7e5a2-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7e5a2-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="7e5a2-106">Пропуск</span><span class="sxs-lookup"><span data-stu-id="7e5a2-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="7e5a2-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="7e5a2-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e5a2-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7e5a2-108">Attributes and elements</span></span>

<span data-ttu-id="7e5a2-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e5a2-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7e5a2-110">Attributes</span></span>

<span data-ttu-id="7e5a2-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e5a2-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7e5a2-112">Child elements</span></span>

|<span data-ttu-id="7e5a2-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e5a2-113">**Element**</span></span>|<span data-ttu-id="7e5a2-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e5a2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e5a2-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="7e5a2-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7e5a2-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e5a2-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7e5a2-117">Parent elements</span></span>

|<span data-ttu-id="7e5a2-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7e5a2-118">**Element**</span></span>|<span data-ttu-id="7e5a2-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7e5a2-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e5a2-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7e5a2-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="7e5a2-121">Определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e5a2-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="7e5a2-122">Remarks</span></span>

<span data-ttu-id="7e5a2-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7e5a2-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e5a2-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7e5a2-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e5a2-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7e5a2-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e5a2-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7e5a2-126">Schema name</span></span>  <br/> |<span data-ttu-id="7e5a2-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7e5a2-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e5a2-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7e5a2-128">Validation file</span></span>  <br/> |<span data-ttu-id="7e5a2-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e5a2-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e5a2-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7e5a2-130">Can be empty</span></span>  <br/> |<span data-ttu-id="7e5a2-131">False</span><span class="sxs-lookup"><span data-stu-id="7e5a2-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e5a2-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7e5a2-132">See also</span></span>



[<span data-ttu-id="7e5a2-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7e5a2-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="7e5a2-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7e5a2-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

