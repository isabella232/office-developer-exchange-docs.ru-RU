---
title: Операция GetUserRetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57c6ff23-5c2c-42ee-824b-5a1b6dafab8c
description: Найдите сведения о веб-служб Exchange GetUserRetentionPolicyTags операции.
ms.openlocfilehash: faf3553c5dd426b522659029bda6819c55f2708d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353233"
---
# <a name="getuserretentionpolicytags-operation"></a><span data-ttu-id="58fd9-103">Операция GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="58fd9-103">GetUserRetentionPolicyTags operation</span></span>

<span data-ttu-id="58fd9-104">Найдите сведения о **GetUserRetentionPolicyTags** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="58fd9-104">Find information about the **GetUserRetentionPolicyTags** EWS operation.</span></span> 
  
<span data-ttu-id="58fd9-105">Операция **GetUserRetentionPolicyTags** возвращает список всех по умолчанию, системная папка и личных тегов, которые связаны с пользователем с помощью политики системы или, были ли применены пользователем.</span><span class="sxs-lookup"><span data-stu-id="58fd9-105">The **GetUserRetentionPolicyTags** operation gets a list of all default, system folder, and personal tags that are associated with a user by means of a system policy or that were applied by the user.</span></span> 
  
<span data-ttu-id="58fd9-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58fd9-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserretentionpolicytags-operation"></a><span data-ttu-id="58fd9-107">С помощью операции GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="58fd9-107">Using the GetUserRetentionPolicyTags operation</span></span>

<span data-ttu-id="58fd9-108">Эта операция возвращает отображаемое имя, идентификатор хранения, срок хранения данных, тип хранения, действие хранения и описание теги и значения для свойства **IsVisible**, **OptedInto**и **IsArchive** .</span><span class="sxs-lookup"><span data-stu-id="58fd9-108">This operation returns the display name, retention ID, retention period, retention type, retention action, and description tags, and the values for the **IsVisible**, **OptedInto**, and **IsArchive** properties.</span></span> 
  
### <a name="getuserretentionpolicytags-operation-soap-headers"></a><span data-ttu-id="58fd9-109">Заголовки SOAP GetUserRetentionPolicyTags операции</span><span class="sxs-lookup"><span data-stu-id="58fd9-109">GetUserRetentionPolicyTags operation SOAP headers</span></span>

<span data-ttu-id="58fd9-110">Операция **GetUserRetentionPolicyTags** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="58fd9-110">The **GetUserRetentionPolicyTags** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="58fd9-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="58fd9-111">**Header name**</span></span>|<span data-ttu-id="58fd9-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58fd9-112">**Element**</span></span>|<span data-ttu-id="58fd9-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58fd9-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="58fd9-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="58fd9-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="58fd9-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="58fd9-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="58fd9-116">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="58fd9-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="58fd9-117">Это применимо к запросу.</span><span class="sxs-lookup"><span data-stu-id="58fd9-117">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58fd9-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="58fd9-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="58fd9-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="58fd9-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="58fd9-120">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="58fd9-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="58fd9-121">Это применимо для ответа.</span><span class="sxs-lookup"><span data-stu-id="58fd9-121">This is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserretentionpolicytags-operation-request-example"></a><span data-ttu-id="58fd9-122">Пример запроса GetUserRetentionPolicyTags операции</span><span class="sxs-lookup"><span data-stu-id="58fd9-122">GetUserRetentionPolicyTags operation request example</span></span>

<span data-ttu-id="58fd9-123">В следующем примере запрос операции **GetUserRetentionPolicyTags** показано, как получить список тегов для текущего пользователя.</span><span class="sxs-lookup"><span data-stu-id="58fd9-123">The following example of a **GetUserRetentionPolicyTags** operation request shows how to get a list of tags for the current user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetUserRetentionPolicyTags />
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="58fd9-124">Запрос SOAP body содержит следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="58fd9-124">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="58fd9-125">GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="58fd9-125">GetUserRetentionPolicyTags</span></span>](getuserretentionpolicytags.md)
    
## <a name="successful-getuserretentionpolicytags-operation-response"></a><span data-ttu-id="58fd9-126">Успешные операции ответа GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="58fd9-126">Successful GetUserRetentionPolicyTags operation response</span></span>

<span data-ttu-id="58fd9-127">В следующем примере показано успешного ответа на запрос операции **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="58fd9-127">The following example shows a successful response to a **GetUserRetentionPolicyTags** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="179" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserRetentionPolicyTagsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <RetentionPolicyTags>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>1 Year Delete</DisplayName>
               <RetentionId>e66252f9-794f-4b36-b55e-d6d95fdf87a3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Personal 1 year move to archive</DisplayName>
               <RetentionId>b2a29464-649c-4174-932b-6aaac9811c89</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Sent Items</DisplayName>
               <RetentionId>b0d32f1b-fbd0-4c1d-ba3e-ddd1086ea1d3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>SentItems</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default 1 year delete</DisplayName>
               <RetentionId>29fc9b9d-98b0-4c01-acf8-3996e2afce98</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Two Year Retention</DisplayName>
               <RetentionId>a1a38957-2557-404e-9f32-53d77c948f62</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description>Use this tag for all items to be retained for two years.</Description>
               <IsVisible>true</IsVisible>
               <OptedInto>true</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default two year move to archive</DisplayName>
               <RetentionId>75bc8dbe-a0e8-4e09-9fa3-fd4c21f49318</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
         </RetentionPolicyTags>
      </GetUserRetentionPolicyTagsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="58fd9-128">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="58fd9-128">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58fd9-129">GetUserRetentionPolicyTagsResponse</span><span class="sxs-lookup"><span data-stu-id="58fd9-129">GetUserRetentionPolicyTagsResponse</span></span>](getuserretentionpolicytagsresponse.md)
    
- [<span data-ttu-id="58fd9-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58fd9-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58fd9-131">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="58fd9-131">RetentionPolicyTags</span></span>](retentionpolicytags.md)
    
- [<span data-ttu-id="58fd9-132">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="58fd9-132">RetentionPolicyTag</span></span>](retentionpolicytag.md)
    
- [<span data-ttu-id="58fd9-133">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="58fd9-133">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58fd9-134">RetentionId</span><span class="sxs-lookup"><span data-stu-id="58fd9-134">RetentionId</span></span>](retentionid.md)
    
- [<span data-ttu-id="58fd9-135">RetentionPeriod</span><span class="sxs-lookup"><span data-stu-id="58fd9-135">RetentionPeriod</span></span>](retentionperiod.md)
    
- [<span data-ttu-id="58fd9-136">Type (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="58fd9-136">Type (ElcFolderType)</span></span>](type-elcfoldertype.md)
    
- [<span data-ttu-id="58fd9-137">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="58fd9-137">RetentionAction</span></span>](retentionaction.md)
    
- [<span data-ttu-id="58fd9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="58fd9-138">Description</span></span>](description.md)
    
- [<span data-ttu-id="58fd9-139">IsVisible</span><span class="sxs-lookup"><span data-stu-id="58fd9-139">IsVisible</span></span>](isvisible.md)
    
- [<span data-ttu-id="58fd9-140">OptedInto</span><span class="sxs-lookup"><span data-stu-id="58fd9-140">OptedInto</span></span>](optedinto.md)
    
- [<span data-ttu-id="58fd9-141">IsArchive</span><span class="sxs-lookup"><span data-stu-id="58fd9-141">IsArchive</span></span>](isarchive.md)
    
## <a name="getuserretentionpolicytags-operation-error-response"></a><span data-ttu-id="58fd9-142">Ошибка операции GetUserRetentionPolicyTags ответа</span><span class="sxs-lookup"><span data-stu-id="58fd9-142">GetUserRetentionPolicyTags operation error response</span></span>

<span data-ttu-id="58fd9-143">Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="58fd9-143">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
