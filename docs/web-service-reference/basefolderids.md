---
title: басефолдеридс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseFolderIds
api_type:
- schema
ms.assetid: bdaa6093-f960-469a-b338-0e75aaa536c6
description: Элемент Басефолдеридс представляет коллекцию папок, которые будут mined для определения содержимого папки поиска.
ms.openlocfilehash: 97159ec1ded685e63aafedfaf90a06eff39adaab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460269"
---
# <a name="basefolderids"></a><span data-ttu-id="39e4d-103">басефолдеридс</span><span class="sxs-lookup"><span data-stu-id="39e4d-103">BaseFolderIds</span></span>

<span data-ttu-id="39e4d-104">Элемент **басефолдеридс** представляет коллекцию папок, которые будут mined для определения содержимого папки поиска.</span><span class="sxs-lookup"><span data-stu-id="39e4d-104">The **BaseFolderIds** element represents the collection of folders that will be mined to determine the contents of a search folder.</span></span> 
  
```xml
<BaseFolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</BaseFolderIds>
```

 <span data-ttu-id="39e4d-105">**нонемптяррайофбасефолдеридстипе**</span><span class="sxs-lookup"><span data-stu-id="39e4d-105">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39e4d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="39e4d-106">Attributes and elements</span></span>

<span data-ttu-id="39e4d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="39e4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39e4d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="39e4d-108">Attributes</span></span>

<span data-ttu-id="39e4d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="39e4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39e4d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="39e4d-110">Child elements</span></span>

|<span data-ttu-id="39e4d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39e4d-111">**Element**</span></span>|<span data-ttu-id="39e4d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39e4d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39e4d-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="39e4d-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="39e4d-114">Содержит идентификатор и ключ изменения папки.</span><span class="sxs-lookup"><span data-stu-id="39e4d-114">Contains the identifier and change key of a folder.</span></span>  <br/> |
|[<span data-ttu-id="39e4d-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="39e4d-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="39e4d-116">Определяет Майкрософт Exchange Server 2007 папок, на которые можно ссылаться по имени.</span><span class="sxs-lookup"><span data-stu-id="39e4d-116">Identifies MicrosoftExchange Server 2007 folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39e4d-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="39e4d-117">Parent elements</span></span>

|<span data-ttu-id="39e4d-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="39e4d-118">**Element**</span></span>|<span data-ttu-id="39e4d-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="39e4d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39e4d-120">сеарчпараметерс</span><span class="sxs-lookup"><span data-stu-id="39e4d-120">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="39e4d-121">Представляет параметры, определяющие папку поиска.</span><span class="sxs-lookup"><span data-stu-id="39e4d-121">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="39e4d-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="39e4d-122">Remarks</span></span>

<span data-ttu-id="39e4d-123">Элемент **басефолдеридс** должен содержать по крайней мере один элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="39e4d-123">The **BaseFolderIds** element must contain at least one [FolderId](folderid.md) or [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="39e4d-124">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="39e4d-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39e4d-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="39e4d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39e4d-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="39e4d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="39e4d-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="39e4d-127">Schema name</span></span>  <br/> |<span data-ttu-id="39e4d-128">Схема Types</span><span class="sxs-lookup"><span data-stu-id="39e4d-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="39e4d-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="39e4d-129">Validation file</span></span>  <br/> |<span data-ttu-id="39e4d-130">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="39e4d-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="39e4d-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="39e4d-131">Can be empty</span></span>  <br/> |<span data-ttu-id="39e4d-132">False</span><span class="sxs-lookup"><span data-stu-id="39e4d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39e4d-133">См. также</span><span class="sxs-lookup"><span data-stu-id="39e4d-133">See also</span></span>



- [<span data-ttu-id="39e4d-134">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39e4d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

