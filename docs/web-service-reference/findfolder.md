---
title: FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: b8a59740-d978-454c-9629-a10792385ba0
description: Элемент FindFolder определяет запрос для поиска папок в почтовом ящике.
ms.openlocfilehash: d41283547c443e38e2e87379a7224df9c89f901d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762559"
---
# <a name="findfolder"></a><span data-ttu-id="6ece1-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="6ece1-103">FindFolder</span></span>

<span data-ttu-id="6ece1-104">Элемент **FindFolder** определяет запрос для поиска папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6ece1-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

 <span data-ttu-id="6ece1-105">**FindFolderType**</span><span class="sxs-lookup"><span data-stu-id="6ece1-105">**FindFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ece1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6ece1-106">Attributes and elements</span></span>

<span data-ttu-id="6ece1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6ece1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ece1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6ece1-108">Attributes</span></span>

|<span data-ttu-id="6ece1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6ece1-109">**Attribute**</span></span>|<span data-ttu-id="6ece1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ece1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ece1-111">Обход</span><span class="sxs-lookup"><span data-stu-id="6ece1-111">Traversal</span></span>  <br/> |<span data-ttu-id="6ece1-112">Определяет, как выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="6ece1-112">Defines how a search is performed.</span></span> <span data-ttu-id="6ece1-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6ece1-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="6ece1-114">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="6ece1-114">Traversal attribute values</span></span>

|<span data-ttu-id="6ece1-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="6ece1-115">**Value**</span></span>|<span data-ttu-id="6ece1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ece1-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6ece1-117">Неполная</span><span class="sxs-lookup"><span data-stu-id="6ece1-117">Shallow</span></span>  <br/> |<span data-ttu-id="6ece1-118">Указывает, что операция FindFolder выполнять поиск только в указанной папке и для возвращения только в папке идентификаторов для элементов, которые не были удалены.</span><span class="sxs-lookup"><span data-stu-id="6ece1-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="6ece1-119">Этот процесс называется частичного обхода.</span><span class="sxs-lookup"><span data-stu-id="6ece1-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="6ece1-120">Глубокое</span><span class="sxs-lookup"><span data-stu-id="6ece1-120">Deep</span></span>  <br/> |<span data-ttu-id="6ece1-121">Указывает, что операция FindFolder для поиска во всех дочерних папках определенного родительской папки и возвращает только в папке идентификаторов для элементов, которые не были удалены.</span><span class="sxs-lookup"><span data-stu-id="6ece1-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="6ece1-122">Этот процесс называется глубину обхода.</span><span class="sxs-lookup"><span data-stu-id="6ece1-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="6ece1-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="6ece1-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="6ece1-124">Указывает, что операция FindFolder для выполнения поиска частичного обхода для удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="6ece1-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6ece1-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6ece1-125">Child elements</span></span>

|<span data-ttu-id="6ece1-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ece1-126">**Element**</span></span>|<span data-ttu-id="6ece1-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ece1-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ece1-128">FolderShape</span><span class="sxs-lookup"><span data-stu-id="6ece1-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="6ece1-129">Задает свойства папки для включения в FindFolder ответа.</span><span class="sxs-lookup"><span data-stu-id="6ece1-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="6ece1-130">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6ece1-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="6ece1-131">Описывает, как выгружаемый элемента сведения возвращаются в ответ FindFolder.</span><span class="sxs-lookup"><span data-stu-id="6ece1-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="6ece1-132">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6ece1-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6ece1-133">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6ece1-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="6ece1-134">Описывает, где начала страничного представления и максимальное число папок, возвращаемых в запросе FindFolder.</span><span class="sxs-lookup"><span data-stu-id="6ece1-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="6ece1-135">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6ece1-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6ece1-136">Ограничения</span><span class="sxs-lookup"><span data-stu-id="6ece1-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="6ece1-137">Задает ограничение или запрос, используемый для фильтрации папок в FindFolder операции.</span><span class="sxs-lookup"><span data-stu-id="6ece1-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="6ece1-138">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6ece1-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="6ece1-139">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="6ece1-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="6ece1-140">Идентифицирует папок для операции FindFolder для поиска.</span><span class="sxs-lookup"><span data-stu-id="6ece1-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ece1-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6ece1-141">Parent elements</span></span>

<span data-ttu-id="6ece1-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="6ece1-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6ece1-143">Замечания</span><span class="sxs-lookup"><span data-stu-id="6ece1-143">Remarks</span></span>

<span data-ttu-id="6ece1-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6ece1-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="6ece1-145">Пример</span><span class="sxs-lookup"><span data-stu-id="6ece1-145">Example</span></span>

<span data-ttu-id="6ece1-146">Пример запроса FindFolder показано, как для формирования запроса, чтобы найти все папки, расположенной в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="6ece1-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="6ece1-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6ece1-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ece1-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6ece1-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6ece1-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6ece1-149">Schema Name</span></span>  <br/> |<span data-ttu-id="6ece1-150">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6ece1-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6ece1-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6ece1-151">Validation File</span></span>  <br/> |<span data-ttu-id="6ece1-152">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6ece1-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ece1-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6ece1-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ece1-154">False</span><span class="sxs-lookup"><span data-stu-id="6ece1-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ece1-155">См. также</span><span class="sxs-lookup"><span data-stu-id="6ece1-155">See also</span></span>



[<span data-ttu-id="6ece1-156">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="6ece1-156">FindFolder operation</span></span>](findfolder-operation.md)

