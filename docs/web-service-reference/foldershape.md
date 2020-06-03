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
ms.openlocfilehash: f841fcc4570604c474387dfa24ec07c9d2784f62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461347"
---
# <a name="foldershape"></a><span data-ttu-id="62655-103">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="62655-103">FolderShape</span></span>

<span data-ttu-id="62655-104">Элемент **фолдершапе** определяет свойства папки, которые необходимо включить в ответ "GetResponse [Folder](getfolder.md)", " [FindFolder](findfolder.md)" и [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="62655-104">The **FolderShape** element identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span> 
  
```xml
<FolderShape>
   <BaseShape/>
   <AdditionalProperties/>
</FolderShape>
```

 <span data-ttu-id="62655-105">**фолдерреспонсешапетипе**</span><span class="sxs-lookup"><span data-stu-id="62655-105">**FolderResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62655-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="62655-106">Attributes and elements</span></span>

<span data-ttu-id="62655-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="62655-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62655-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="62655-108">Attributes</span></span>

<span data-ttu-id="62655-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="62655-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62655-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="62655-110">Child elements</span></span>

|<span data-ttu-id="62655-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62655-111">**Element**</span></span>|<span data-ttu-id="62655-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62655-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62655-113">басешапе</span><span class="sxs-lookup"><span data-stu-id="62655-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="62655-114">Определяет базовую конфигурацию свойств, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="62655-114">Identifies the basic configuration of properties to return in a response.</span></span>  <br/> |
|[<span data-ttu-id="62655-115">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="62655-115">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="62655-116">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="62655-116">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62655-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="62655-117">Parent elements</span></span>

|<span data-ttu-id="62655-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62655-118">**Element**</span></span>|<span data-ttu-id="62655-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62655-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62655-120">FindFolder</span><span class="sxs-lookup"><span data-stu-id="62655-120">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="62655-121">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="62655-121">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="62655-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="62655-122">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
|[<span data-ttu-id="62655-123">GetFolder</span><span class="sxs-lookup"><span data-stu-id="62655-123">GetFolder</span></span>](getfolder.md) <br/> |<span data-ttu-id="62655-124">Определяет запрос на получение папки из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="62655-124">Defines a request to get a folder from the Exchange store.</span></span>  <br/> <span data-ttu-id="62655-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="62655-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetFolder` <br/> |
|[<span data-ttu-id="62655-126">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="62655-126">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md) <br/> |<span data-ttu-id="62655-127">Определяет запрос на синхронизацию иерархии папок в клиенте.</span><span class="sxs-lookup"><span data-stu-id="62655-127">Defines a request to synchronize a folder hierarchy on a client.</span></span>  <br/> <span data-ttu-id="62655-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="62655-128">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderHierarchy` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="62655-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="62655-129">Remarks</span></span>

<span data-ttu-id="62655-130">Элемент **фолдершапе** является обязательным дочерним элементом элемента [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="62655-130">The **FolderShape** element is a required child element of the [FindFolder](findfolder.md) element.</span></span> 
  
<span data-ttu-id="62655-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="62655-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="62655-132">Пример</span><span class="sxs-lookup"><span data-stu-id="62655-132">Example</span></span>

<span data-ttu-id="62655-133">В приведенном ниже примере запроса показано, как найти все папки, расположенные на первом уровне папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="62655-133">The following example of a request demonstrates how to find all folders located in the first level of the Inbox folder.</span></span>
  
```
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

## <a name="element-information"></a><span data-ttu-id="62655-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="62655-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62655-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="62655-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="62655-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="62655-136">Schema Name</span></span>  <br/> |<span data-ttu-id="62655-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="62655-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="62655-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="62655-138">Validation File</span></span>  <br/> |<span data-ttu-id="62655-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="62655-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="62655-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="62655-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="62655-141">False</span><span class="sxs-lookup"><span data-stu-id="62655-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62655-142">См. также</span><span class="sxs-lookup"><span data-stu-id="62655-142">See also</span></span>



[<span data-ttu-id="62655-143">FindFolder</span><span class="sxs-lookup"><span data-stu-id="62655-143">FindFolder</span></span>](findfolder.md)

