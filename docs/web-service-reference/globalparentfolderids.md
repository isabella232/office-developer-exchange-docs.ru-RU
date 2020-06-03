---
title: глобалпарентфолдеридс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f5fcbcb-05ed-462a-99cf-a6b112a4aef6
description: Элемент Глобалпарентфолдеридс указывает идентификаторы глобальных родительских папок.
ms.openlocfilehash: 11c520fa0f4a1ed6d6c9d694b407e39cd036b9cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459099"
---
# <a name="globalparentfolderids"></a><span data-ttu-id="4cd3b-103">глобалпарентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="4cd3b-103">GlobalParentFolderIds</span></span>

<span data-ttu-id="4cd3b-104">Элемент **глобалпарентфолдеридс** указывает идентификаторы глобальных родительских папок.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-104">The **GlobalParentFolderIds** element specifies the identifiers of the global parent folders.</span></span> 
  
```XML
<GlobalParentFolderIds>
    <FolderId/>
    <DistinguishedFolderId/>
</GlobalParentFolderIds>
```

 <span data-ttu-id="4cd3b-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="4cd3b-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cd3b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4cd3b-106">Attributes and elements</span></span>

<span data-ttu-id="4cd3b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cd3b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4cd3b-108">Attributes</span></span>

<span data-ttu-id="4cd3b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cd3b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4cd3b-110">Child elements</span></span>

|<span data-ttu-id="4cd3b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cd3b-111">**Element**</span></span>|<span data-ttu-id="4cd3b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cd3b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd3b-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="4cd3b-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="4cd3b-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="4cd3b-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="4cd3b-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="4cd3b-116">Определяет папки, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-116">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cd3b-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4cd3b-117">Parent elements</span></span>

|<span data-ttu-id="4cd3b-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cd3b-118">**Element**</span></span>|<span data-ttu-id="4cd3b-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cd3b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd3b-120">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4cd3b-120">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="4cd3b-121">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-121">Represents a single conversation.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4cd3b-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="4cd3b-122">Remarks</span></span>

<span data-ttu-id="4cd3b-123">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4cd3b-124">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd3b-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cd3b-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4cd3b-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cd3b-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4cd3b-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4cd3b-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4cd3b-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4cd3b-128">Схема типа</span><span class="sxs-lookup"><span data-stu-id="4cd3b-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4cd3b-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4cd3b-129">Validation File</span></span>  <br/> |<span data-ttu-id="4cd3b-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4cd3b-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4cd3b-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4cd3b-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4cd3b-132">См. также</span><span class="sxs-lookup"><span data-stu-id="4cd3b-132">See also</span></span>



- [<span data-ttu-id="4cd3b-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4cd3b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

