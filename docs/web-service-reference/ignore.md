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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833858"
---
# <a name="ignore"></a><span data-ttu-id="7c320-103">Пропуск</span><span class="sxs-lookup"><span data-stu-id="7c320-103">Ignore</span></span>

<span data-ttu-id="7c320-104">Элемент **Игнорировать** определяет элементы, чтобы пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="7c320-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="7c320-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7c320-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="7c320-106">Пропуск</span><span class="sxs-lookup"><span data-stu-id="7c320-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="7c320-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="7c320-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c320-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c320-108">Attributes and elements</span></span>

<span data-ttu-id="7c320-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7c320-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c320-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c320-110">Attributes</span></span>

<span data-ttu-id="7c320-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c320-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c320-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c320-112">Child elements</span></span>

|<span data-ttu-id="7c320-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c320-113">**Element**</span></span>|<span data-ttu-id="7c320-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c320-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c320-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="7c320-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7c320-116">Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c320-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c320-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c320-117">Parent elements</span></span>

|<span data-ttu-id="7c320-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c320-118">**Element**</span></span>|<span data-ttu-id="7c320-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c320-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c320-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7c320-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="7c320-121">Определяет запрос для синхронизации элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c320-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c320-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c320-122">Remarks</span></span>

<span data-ttu-id="7c320-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7c320-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c320-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c320-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c320-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c320-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c320-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c320-126">Schema name</span></span>  <br/> |<span data-ttu-id="7c320-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7c320-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7c320-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c320-128">Validation file</span></span>  <br/> |<span data-ttu-id="7c320-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c320-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c320-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c320-130">Can be empty</span></span>  <br/> |<span data-ttu-id="7c320-131">False</span><span class="sxs-lookup"><span data-stu-id="7c320-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c320-132">См. также</span><span class="sxs-lookup"><span data-stu-id="7c320-132">See also</span></span>



[<span data-ttu-id="7c320-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="7c320-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="7c320-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c320-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

