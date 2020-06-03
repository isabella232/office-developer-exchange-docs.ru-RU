---
title: синкфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderId
api_type:
- schema
ms.assetid: 3645fa03-236d-4e5f-b8b9-5d98f7f35fa2
description: Элемент Синкфолдерид представляет папку, содержащую синхронизируемые элементы.
ms.openlocfilehash: 35b66579116a00d27df722629ff980471ca0272e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530298"
---
# <a name="syncfolderid"></a><span data-ttu-id="d65dc-103">синкфолдерид</span><span class="sxs-lookup"><span data-stu-id="d65dc-103">SyncFolderId</span></span>

<span data-ttu-id="d65dc-104">Элемент **синкфолдерид** представляет папку, содержащую синхронизируемые элементы.</span><span class="sxs-lookup"><span data-stu-id="d65dc-104">The **SyncFolderId** element represents the folder that contains the items to synchronize.</span></span> 
  
```xml
<SyncFolderId>
   <FolderId/>
</SyncFolderId>
```

```xml
<SyncFolderId>
   <DistinguishedFolderId/> 
</SyncFolderId>
```

<span data-ttu-id="d65dc-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="d65dc-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d65dc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d65dc-106">Attributes and elements</span></span>

<span data-ttu-id="d65dc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d65dc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d65dc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d65dc-108">Attributes</span></span>

<span data-ttu-id="d65dc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d65dc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d65dc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d65dc-110">Child elements</span></span>

|<span data-ttu-id="d65dc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d65dc-111">**Element**</span></span>|<span data-ttu-id="d65dc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d65dc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d65dc-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="d65dc-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d65dc-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="d65dc-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="d65dc-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="d65dc-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="d65dc-116">Определяет Майкрософт Exchange Server 2007 папок, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="d65dc-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d65dc-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d65dc-117">Parent elements</span></span>

|<span data-ttu-id="d65dc-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d65dc-118">**Element**</span></span>|<span data-ttu-id="d65dc-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d65dc-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d65dc-120">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="d65dc-120">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="d65dc-121">Определяет запрос на синхронизацию иерархии папок в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d65dc-121">Defines a request to synchronize a folder hierarchy in an Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="d65dc-122">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="d65dc-122">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="d65dc-123">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d65dc-123">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d65dc-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="d65dc-124">Remarks</span></span>

<span data-ttu-id="d65dc-125">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d65dc-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d65dc-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d65dc-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d65dc-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d65dc-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d65dc-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d65dc-128">Schema name</span></span>  <br/> |<span data-ttu-id="d65dc-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d65dc-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d65dc-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d65dc-130">Validation file</span></span>  <br/> |<span data-ttu-id="d65dc-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d65dc-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d65dc-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d65dc-132">Can be empty</span></span>  <br/> |<span data-ttu-id="d65dc-133">False</span><span class="sxs-lookup"><span data-stu-id="d65dc-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d65dc-134">См. также</span><span class="sxs-lookup"><span data-stu-id="d65dc-134">See also</span></span>

- [<span data-ttu-id="d65dc-135">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="d65dc-135">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="d65dc-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d65dc-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

