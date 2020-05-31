---
title: фолдершапе
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
description: Элемент Фолдершапе определяет свойства папки, которые необходимо включить в ответ "GetResponse Folder", "FindFolder" и SyncFolderHierarchy.
ms.openlocfilehash: 8ebdd70ef13ee9f0cce9020b9212576cba782be4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762640"
---
# <a name="foldershape"></a><span data-ttu-id="166ef-103">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="166ef-103">FolderShape</span></span>

<span data-ttu-id="166ef-104">Элемент **фолдершапе** определяет свойства папки, которые необходимо включить в ответ "GetResponse [Folder](getfolder.md)", " [FindFolder](findfolder.md)" и [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="166ef-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="166ef-105">**фолдерреспонсешапетипе**</span><span class="sxs-lookup"><span data-stu-id="166ef-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="166ef-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="166ef-106">Attributes and elements</span></span>

<span data-ttu-id="166ef-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="166ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="166ef-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="166ef-108">Attributes</span></span>

<span data-ttu-id="166ef-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="166ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="166ef-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="166ef-110">Child elements</span></span>

|<span data-ttu-id="166ef-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="166ef-111">**Element**</span></span>|<span data-ttu-id="166ef-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="166ef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="166ef-113">басешапе</span><span class="sxs-lookup"><span data-stu-id="166ef-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="166ef-114">Определяет базовую конфигурацию свойств, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="166ef-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="166ef-115">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="166ef-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="166ef-116">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="166ef-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="166ef-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="166ef-117">Parent elements</span></span>

|<span data-ttu-id="166ef-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="166ef-118">**Element**</span></span>|<span data-ttu-id="166ef-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="166ef-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="166ef-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="166ef-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="166ef-121">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="166ef-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="166ef-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="166ef-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="166ef-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="166ef-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="166ef-124">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="166ef-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="166ef-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="166ef-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="166ef-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="166ef-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="166ef-127">Определяет запрос на синхронизацию иерархии папок в клиенте.</span><span class="sxs-lookup"><span data-stu-id="166ef-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="166ef-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="166ef-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="166ef-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="166ef-129">Remarks</span></span>

<span data-ttu-id="166ef-130">Элемент **фолдершапе** является обязательным дочерним элементом элемента [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="166ef-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="166ef-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="166ef-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="166ef-132">Пример</span><span class="sxs-lookup"><span data-stu-id="166ef-132">Example</span></span>

<span data-ttu-id="166ef-133">В приведенном ниже примере запроса показано, как найти все папки, расположенные на первом уровне папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="166ef-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="166ef-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="166ef-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="166ef-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="166ef-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="166ef-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="166ef-136">Schema Name</span></span>  <br/> |<span data-ttu-id="166ef-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="166ef-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="166ef-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="166ef-138">Validation File</span></span>  <br/> |<span data-ttu-id="166ef-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="166ef-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="166ef-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="166ef-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="166ef-141">False</span><span class="sxs-lookup"><span data-stu-id="166ef-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="166ef-142">См. также</span><span class="sxs-lookup"><span data-stu-id="166ef-142">See also</span></span>



[<span data-ttu-id="166ef-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="166ef-143">FindFolder</span></span>](findfolder.md)

