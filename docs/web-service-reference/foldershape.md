---
title: FolderShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderShape
api_type:
- schema
ms.assetid: 244f4f46-a33d-4764-92e3-1bddb4dc6a49
description: Элемент FolderShape определяет свойства папки для включения в GetFolder, FindFolder или SyncFolderHierarchy ответа.
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762640"
---
# <a name="foldershape"></a><span data-ttu-id="ce7e4-103">FolderShape</span><span class="sxs-lookup"><span data-stu-id="ce7e4-103">FolderShape</span></span>

<span data-ttu-id="ce7e4-104">Элемент **FolderShape** определяет свойства папки для включения в [GetFolder](getfolder.md), [FindFolder](findfolder.md)или [SyncFolderHierarchy](syncfolderhierarchy.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="ce7e4-105">**FolderResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="ce7e4-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ce7e4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ce7e4-106">Attributes and elements</span></span>

<span data-ttu-id="ce7e4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ce7e4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ce7e4-108">Attributes</span></span>

<span data-ttu-id="ce7e4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ce7e4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ce7e4-110">Child elements</span></span>

|<span data-ttu-id="ce7e4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce7e4-111">**Element**</span></span>|<span data-ttu-id="ce7e4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce7e4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce7e4-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ce7e4-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="ce7e4-114">Определяет базовую конфигурацию свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="ce7e4-115">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="ce7e4-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="ce7e4-116">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ce7e4-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ce7e4-117">Parent elements</span></span>

|<span data-ttu-id="ce7e4-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ce7e4-118">**Element**</span></span>|<span data-ttu-id="ce7e4-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ce7e4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ce7e4-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ce7e4-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="ce7e4-121">Определяет запрос для определения папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="ce7e4-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="ce7e4-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="ce7e4-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="ce7e4-124">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="ce7e4-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="ce7e4-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="ce7e4-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="ce7e4-127">Определяет запрос для синхронизации иерархии папок на клиенте.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="ce7e4-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ce7e4-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="ce7e4-129">Remarks</span></span>

<span data-ttu-id="ce7e4-130">Элемент **FolderShape** является обязательным дочерним элементом элемента [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ce7e4-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="ce7e4-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ce7e4-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ce7e4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="ce7e4-132">Example</span></span>

<span data-ttu-id="ce7e4-133">Следующий пример запроса показано, как найти все папки, расположенной в первый уровень папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="ce7e4-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="ce7e4-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ce7e4-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ce7e4-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ce7e4-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ce7e4-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ce7e4-136">Schema Name</span></span>  <br/> |<span data-ttu-id="ce7e4-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ce7e4-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ce7e4-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ce7e4-138">Validation File</span></span>  <br/> |<span data-ttu-id="ce7e4-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ce7e4-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ce7e4-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ce7e4-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="ce7e4-141">False</span><span class="sxs-lookup"><span data-stu-id="ce7e4-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ce7e4-142">См. также</span><span class="sxs-lookup"><span data-stu-id="ce7e4-142">See also</span></span>



[<span data-ttu-id="ce7e4-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ce7e4-143">FindFolder</span></span>](findfolder.md)

