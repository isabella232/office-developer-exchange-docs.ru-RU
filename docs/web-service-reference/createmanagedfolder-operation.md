---
title: Операция CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: Операция CreateManagedFolder создает управляемых папок в хранилище Exchange.
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761909"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="5a2e1-103">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="5a2e1-104">Операция CreateManagedFolder создает управляемых папок в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="5a2e1-105">С помощью операции CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="5a2e1-106">Операция CreateManagedFolder добавляет настраиваемой управляемой папки почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="5a2e1-107">Командлет командной консоли Exchange **Get-ManagedFolder** найти доступные управляемые папки для добавления.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="5a2e1-108">Несмотря на то, что этот командлет возвращает управляемые настраиваемые папки и управляемые папки по умолчанию, только управляемые настраиваемые папки можно добавить.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="5a2e1-109">Управляемые настраиваемые папки, идентифицируются по типу папки ManagedCustomFolder.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="5a2e1-110">Пространство имен System.DirectoryServices также содержит типы, которые можно использовать для получения имен доступных управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5a2e1-111">Нельзя использовать веб-служб Exchange для поиска имен доступен управляемые папки для добавления к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="5a2e1-112">Операции FindFolder и GetFolder можно использовать для доступа к управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="5a2e1-113">FindFolder используется для поиска папок в указанной родительской папки.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="5a2e1-114">Можно использовать, чтобы управляемые папки для обнаружения в папке, прежде чем пытаться добавить дубликат настраиваемую управляемую папку на том же каталоге.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="5a2e1-115">GetFolder используется после операции FindFolder для получения дополнительных сведений о настраиваемой управляемой папки.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5a2e1-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="5a2e1-116">Remarks</span></span>

<span data-ttu-id="5a2e1-117">Сведения о настройке политики управления записями обмена сообщениями Узнайте, [как создать политику почтовых ящиков управляемых папок](http://go.microsoft.com/fwlink/?LinkId=100975).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](http://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="5a2e1-118">Сведения о том, как удалить управляемые настраиваемые папки из почтового ящика можно [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).</span><span class="sxs-lookup"><span data-stu-id="5a2e1-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="5a2e1-119">Пример запроса CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="5a2e1-120">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e1-120">Description</span></span>

<span data-ttu-id="5a2e1-121">В следующем примере запрос CreateManagedFolder показано, как для добавления управляемых папок с именем Test управляемых папок для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5a2e1-122">Передача прав доступа можно также использовать для добавления настраиваемых управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5a2e1-123">Программа</span><span class="sxs-lookup"><span data-stu-id="5a2e1-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5a2e1-124">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="5a2e1-124">Request elements</span></span>

<span data-ttu-id="5a2e1-125">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5a2e1-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5a2e1-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="5a2e1-127">FolderNames</span><span class="sxs-lookup"><span data-stu-id="5a2e1-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="5a2e1-128">Имя папки</span><span class="sxs-lookup"><span data-stu-id="5a2e1-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="5a2e1-129">Чтобы найти другие параметры для запроса CreateManagedFolder операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5a2e1-130">Запустите в элементе [CreateManagedFolder](createmanagedfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2e1-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="5a2e1-131">Успешного ответа CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="5a2e1-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e1-132">Description</span></span>

<span data-ttu-id="5a2e1-133">В следующем примере кода показано успешного ответа на запрос CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5a2e1-134">Значения атрибута **Id** и **ChangeKey** URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5a2e1-135">Программа</span><span class="sxs-lookup"><span data-stu-id="5a2e1-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="5a2e1-136">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="5a2e1-136">Successful response elements</span></span>

<span data-ttu-id="5a2e1-137">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5a2e1-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="5a2e1-138">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5a2e1-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="5a2e1-139">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a2e1-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a2e1-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5a2e1-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="5a2e1-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a2e1-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5a2e1-142">Папки</span><span class="sxs-lookup"><span data-stu-id="5a2e1-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5a2e1-143">Folder</span><span class="sxs-lookup"><span data-stu-id="5a2e1-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="5a2e1-144">FolderId</span><span class="sxs-lookup"><span data-stu-id="5a2e1-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="5a2e1-145">Чтобы найти другие параметры сообщений ответа CreateManagedFolder операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5a2e1-146">Запустите в элементе [CreateManagedFolderResponse](createmanagedfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="5a2e1-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="5a2e1-147">Ошибка CreateManagedFolder ответа</span><span class="sxs-lookup"><span data-stu-id="5a2e1-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="5a2e1-148">Описание</span><span class="sxs-lookup"><span data-stu-id="5a2e1-148">Description</span></span>

<span data-ttu-id="5a2e1-149">В следующем примере кода показано ошибочный ответ на запрос CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="5a2e1-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a2e1-150">Программа</span><span class="sxs-lookup"><span data-stu-id="5a2e1-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="5a2e1-151">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="5a2e1-151">Error response elements</span></span>

<span data-ttu-id="5a2e1-152">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5a2e1-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5a2e1-153">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5a2e1-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="5a2e1-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5a2e1-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5a2e1-155">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5a2e1-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="5a2e1-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="5a2e1-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5a2e1-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5a2e1-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5a2e1-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5a2e1-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5a2e1-159">Папки</span><span class="sxs-lookup"><span data-stu-id="5a2e1-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="5a2e1-160">См. также</span><span class="sxs-lookup"><span data-stu-id="5a2e1-160">See also</span></span>



[<span data-ttu-id="5a2e1-161">GetFolder Operation</span><span class="sxs-lookup"><span data-stu-id="5a2e1-161">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="5a2e1-162">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="5a2e1-162">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="5a2e1-163">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="5a2e1-163">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="5a2e1-164">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="5a2e1-164">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

