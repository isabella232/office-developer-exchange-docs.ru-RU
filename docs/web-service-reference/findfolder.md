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
description: Элемент FindFolder определяет запрос на поиск папок в почтовом ящике.
ms.openlocfilehash: 248047206a661afe723543e52c51b57847148423
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462579"
---
# <a name="findfolder"></a><span data-ttu-id="49c49-103">FindFolder</span><span class="sxs-lookup"><span data-stu-id="49c49-103">FindFolder</span></span>

<span data-ttu-id="49c49-104">Элемент **FindFolder** определяет запрос на поиск папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="49c49-104">The **FindFolder** element defines a request to find folders in a mailbox.</span></span> 
  
```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <IndexedPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

```xml
<FindFolder Traversal="Shallow/Deep/SoftDeleted">
   <FolderShape/>
   <FractionalPageFolderView/>
   <Restriction/>
   <ParentFolderIds/>
</FindFolder>
```

<span data-ttu-id="49c49-105">**финдфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="49c49-105">**FindFolderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="49c49-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49c49-106">Attributes and elements</span></span>

<span data-ttu-id="49c49-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="49c49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49c49-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49c49-108">Attributes</span></span>

|<span data-ttu-id="49c49-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="49c49-109">**Attribute**</span></span>|<span data-ttu-id="49c49-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49c49-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49c49-111">Обход</span><span class="sxs-lookup"><span data-stu-id="49c49-111">Traversal</span></span>  <br/> |<span data-ttu-id="49c49-112">Определяет способ выполнения поиска.</span><span class="sxs-lookup"><span data-stu-id="49c49-112">Defines how a search is performed.</span></span> <span data-ttu-id="49c49-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="49c49-113">This attribute is required.</span></span>  <br/> |
   
#### <a name="traversal-attribute-values"></a><span data-ttu-id="49c49-114">Значения атрибутов обхода</span><span class="sxs-lookup"><span data-stu-id="49c49-114">Traversal attribute values</span></span>

|<span data-ttu-id="49c49-115">**Значение**</span><span class="sxs-lookup"><span data-stu-id="49c49-115">**Value**</span></span>|<span data-ttu-id="49c49-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49c49-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49c49-117">Поверхност</span><span class="sxs-lookup"><span data-stu-id="49c49-117">Shallow</span></span>  <br/> |<span data-ttu-id="49c49-118">Инструктирует операцию FindFolder для поиска только в идентифицированной папке и возврата только идентификаторов папок для элементов, которые не были удалены.</span><span class="sxs-lookup"><span data-stu-id="49c49-118">Instructs the FindFolder operation to search only the identified folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="49c49-119">Это называется неповерхностным обходом.</span><span class="sxs-lookup"><span data-stu-id="49c49-119">This is called a shallow traversal.</span></span>  <br/> |
|<span data-ttu-id="49c49-120">Углублен</span><span class="sxs-lookup"><span data-stu-id="49c49-120">Deep</span></span>  <br/> |<span data-ttu-id="49c49-121">Инструктирует операцию FindFolder для поиска во всех дочерних папках указанной родительской папки и возврата только идентификаторов папок для элементов, которые не были удалены.</span><span class="sxs-lookup"><span data-stu-id="49c49-121">Instructs the FindFolder operation to search in all child folders of the identified parent folder and to return only the folder IDs for items that have not been deleted.</span></span> <span data-ttu-id="49c49-122">Это называется глубоким обходом.</span><span class="sxs-lookup"><span data-stu-id="49c49-122">This is called a deep traversal.</span></span>  <br/> |
|<span data-ttu-id="49c49-123">SoftDeleted</span><span class="sxs-lookup"><span data-stu-id="49c49-123">SoftDeleted</span></span>  <br/> |<span data-ttu-id="49c49-124">Инструктирует операцию FindFolder для выполнения неполном обходного поиска для удаленных элементов.</span><span class="sxs-lookup"><span data-stu-id="49c49-124">Instructs the FindFolder operation to perform a shallow traversal search for deleted items.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="49c49-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49c49-125">Child elements</span></span>

|<span data-ttu-id="49c49-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49c49-126">**Element**</span></span>|<span data-ttu-id="49c49-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49c49-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49c49-128">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="49c49-128">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="49c49-129">Определяет свойства папки, включаемые в отклике FindFolder.</span><span class="sxs-lookup"><span data-stu-id="49c49-129">Identifies the folder properties to include in a FindFolder response.</span></span>  <br/> |
|[<span data-ttu-id="49c49-130">индекседпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="49c49-130">IndexedPageFolderView</span></span>](indexedpagefolderview.md) <br/> |<span data-ttu-id="49c49-131">Описывает, как возвращаются сведения о страничном элементе в отклике FindFolder.</span><span class="sxs-lookup"><span data-stu-id="49c49-131">Describes how paged item information is returned in a FindFolder response.</span></span> <span data-ttu-id="49c49-132">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="49c49-132">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="49c49-133">фрактионалпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="49c49-133">FractionalPageFolderView</span></span>](fractionalpagefolderview.md) <br/> |<span data-ttu-id="49c49-134">Описывает, где начинается страничное представление, и максимальное количество папок, возвращаемых в запросе FindFolder.</span><span class="sxs-lookup"><span data-stu-id="49c49-134">Describes where the paged view starts and the maximum number of folders returned in a FindFolder request.</span></span> <span data-ttu-id="49c49-135">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="49c49-135">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="49c49-136">Restriction</span><span class="sxs-lookup"><span data-stu-id="49c49-136">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="49c49-137">Определяет ограничение или запрос, используемый для фильтрации папок в операции FindFolder.</span><span class="sxs-lookup"><span data-stu-id="49c49-137">Defines a restriction or query that is used to filter folders in a FindFolder operation.</span></span> <span data-ttu-id="49c49-138">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="49c49-138">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="49c49-139">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="49c49-139">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="49c49-140">Определяет папки для поиска в операции FindFolder.</span><span class="sxs-lookup"><span data-stu-id="49c49-140">Identifies folders for the FindFolder operation to search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49c49-141">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49c49-141">Parent elements</span></span>

<span data-ttu-id="49c49-142">Нет.</span><span class="sxs-lookup"><span data-stu-id="49c49-142">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49c49-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="49c49-143">Remarks</span></span>

<span data-ttu-id="49c49-144">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="49c49-144">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="49c49-145">Пример</span><span class="sxs-lookup"><span data-stu-id="49c49-145">Example</span></span>

<span data-ttu-id="49c49-146">В следующем примере запроса FindFolder показано, как сформировать запрос на поиск всех папок, расположенных в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="49c49-146">The following example of a FindFolder request shows how to form a request to find all the folders located in an Inbox.</span></span>
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a><span data-ttu-id="49c49-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49c49-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49c49-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49c49-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49c49-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49c49-149">Schema Name</span></span>  <br/> |<span data-ttu-id="49c49-150">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="49c49-150">Messages schema</span></span>  <br/> |
|<span data-ttu-id="49c49-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49c49-151">Validation File</span></span>  <br/> |<span data-ttu-id="49c49-152">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="49c49-152">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49c49-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49c49-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="49c49-154">False</span><span class="sxs-lookup"><span data-stu-id="49c49-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49c49-155">См. также</span><span class="sxs-lookup"><span data-stu-id="49c49-155">See also</span></span>

- [<span data-ttu-id="49c49-156">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="49c49-156">FindFolder operation</span></span>](findfolder-operation.md)

