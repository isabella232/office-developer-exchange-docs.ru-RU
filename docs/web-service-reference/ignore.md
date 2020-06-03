---
title: Игнорировать
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
description: Элемент Ignore определяет элементы, которые необходимо пропустить во время синхронизации.
ms.openlocfilehash: b65d11d8c7655279dac0e7d3cbd13f8a9317540c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458574"
---
# <a name="ignore"></a><span data-ttu-id="bd211-103">Игнорировать</span><span class="sxs-lookup"><span data-stu-id="bd211-103">Ignore</span></span>

<span data-ttu-id="bd211-104">Элемент **Ignore** определяет элементы, которые необходимо пропустить во время синхронизации.</span><span class="sxs-lookup"><span data-stu-id="bd211-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="bd211-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="bd211-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="bd211-106">Ignore</span><span class="sxs-lookup"><span data-stu-id="bd211-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="bd211-107">**аррайофбасеитемидстипе**</span><span class="sxs-lookup"><span data-stu-id="bd211-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd211-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd211-108">Attributes and elements</span></span>

<span data-ttu-id="bd211-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bd211-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd211-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd211-110">Attributes</span></span>

<span data-ttu-id="bd211-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bd211-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd211-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd211-112">Child elements</span></span>

|<span data-ttu-id="bd211-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd211-113">**Element**</span></span>|<span data-ttu-id="bd211-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd211-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd211-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="bd211-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bd211-116">Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd211-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd211-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd211-117">Parent elements</span></span>

|<span data-ttu-id="bd211-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd211-118">**Element**</span></span>|<span data-ttu-id="bd211-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd211-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd211-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="bd211-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="bd211-121">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="bd211-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd211-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="bd211-122">Remarks</span></span>

<span data-ttu-id="bd211-123">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bd211-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd211-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd211-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd211-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd211-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd211-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd211-126">Schema name</span></span>  <br/> |<span data-ttu-id="bd211-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="bd211-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd211-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd211-128">Validation file</span></span>  <br/> |<span data-ttu-id="bd211-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bd211-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd211-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd211-130">Can be empty</span></span>  <br/> |<span data-ttu-id="bd211-131">False</span><span class="sxs-lookup"><span data-stu-id="bd211-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd211-132">См. также</span><span class="sxs-lookup"><span data-stu-id="bd211-132">See also</span></span>



[<span data-ttu-id="bd211-133">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="bd211-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="bd211-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd211-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

