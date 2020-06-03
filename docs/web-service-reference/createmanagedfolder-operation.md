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
description: Операция CreateManagedFolder создает управляемую папку в хранилище Exchange.
ms.openlocfilehash: 779c730b55b9b441644108a6837f9e22d39cc2f4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44444595"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="60ecd-103">Операция CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="60ecd-104">Операция CreateManagedFolder создает управляемую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="60ecd-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="60ecd-105">Использование операции CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="60ecd-106">Операция CreateManagedFolder добавляет настраиваемую управляемую папку в почтовый ящик пользователя.</span><span class="sxs-lookup"><span data-stu-id="60ecd-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="60ecd-107">С помощью командлета **Get – ManagedFolder** в командной консоли Exchange можно найти доступные управляемые папки для добавления.</span><span class="sxs-lookup"><span data-stu-id="60ecd-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="60ecd-108">Несмотря на то, что этот командлет возвращает как управляемые настраиваемые папки, так и управляемые папки по умолчанию, можно добавлять только настраиваемые папки с управляемыми папками.</span><span class="sxs-lookup"><span data-stu-id="60ecd-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="60ecd-109">Управляемые настраиваемые папки определяются типом папки Манажедкустомфолдер.</span><span class="sxs-lookup"><span data-stu-id="60ecd-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="60ecd-110">Пространство имен System. DirectoryServices также включает типы, которые можно использовать для обнаружения имен доступных управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="60ecd-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="60ecd-111">Веб-службы Exchange невозможно использовать для поиска имен доступных управляемых папок, добавляемых в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="60ecd-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="60ecd-112">Вы можете использовать операции FindFolder и a Folder для доступа к управляемым папкам.</span><span class="sxs-lookup"><span data-stu-id="60ecd-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="60ecd-113">FindFolder используется для поиска папок в указанной родительской папке.</span><span class="sxs-lookup"><span data-stu-id="60ecd-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="60ecd-114">Это можно использовать для обнаружения управляемых папок в папке перед попыткой добавить дублирующую управляемую настраиваемую папку в тот же каталог.</span><span class="sxs-lookup"><span data-stu-id="60ecd-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="60ecd-115">"-Папка" используется после операции FindFolder для получения дополнительных сведений об управляемой настраиваемой папке.</span><span class="sxs-lookup"><span data-stu-id="60ecd-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60ecd-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="60ecd-116">Remarks</span></span>

<span data-ttu-id="60ecd-117">Сведения о том, как настроить политику управления записями сообщений (управления ЗАПИСЯМИ сообщений), приведены [в статье Создание политики почтовых ящиков управляемых папок](https://go.microsoft.com/fwlink/?LinkId=100975).</span><span class="sxs-lookup"><span data-stu-id="60ecd-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](https://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="60ecd-118">Сведения об удалении управляемых настраиваемых папок из почтового ящика можно найти в статье [Remove – ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).</span><span class="sxs-lookup"><span data-stu-id="60ecd-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](https://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="60ecd-119">Пример запроса CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="60ecd-120">Description</span><span class="sxs-lookup"><span data-stu-id="60ecd-120">Description</span></span>

<span data-ttu-id="60ecd-121">В приведенном ниже примере запроса CreateManagedFolder показано, как добавить управляемую папку с именем Test Managed Folder в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="60ecd-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="60ecd-122">Вы также можете использовать делегированный доступ для добавления настраиваемых управляемых папок.</span><span class="sxs-lookup"><span data-stu-id="60ecd-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="60ecd-123">Код</span><span class="sxs-lookup"><span data-stu-id="60ecd-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="60ecd-124">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="60ecd-124">Request elements</span></span>

<span data-ttu-id="60ecd-125">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="60ecd-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="60ecd-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="60ecd-127">фолдернамес</span><span class="sxs-lookup"><span data-stu-id="60ecd-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="60ecd-128">FolderName</span><span class="sxs-lookup"><span data-stu-id="60ecd-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="60ecd-129">Чтобы найти другие параметры сообщения Request операции CreateManagedFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="60ecd-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="60ecd-130">Начните с элемента [CreateManagedFolder](createmanagedfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="60ecd-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="60ecd-131">Успешный ответ CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="60ecd-132">Description</span><span class="sxs-lookup"><span data-stu-id="60ecd-132">Description</span></span>

<span data-ttu-id="60ecd-133">В следующем примере кода показан успешный ответ на запрос CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="60ecd-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="60ecd-134">Значения атрибута **ID** и **чанжекэй** были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="60ecd-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="60ecd-135">Код</span><span class="sxs-lookup"><span data-stu-id="60ecd-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="60ecd-136">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="60ecd-136">Successful response elements</span></span>

<span data-ttu-id="60ecd-137">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="60ecd-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="60ecd-138">креатеманажедфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="60ecd-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="60ecd-139">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="60ecd-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="60ecd-140">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="60ecd-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="60ecd-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="60ecd-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="60ecd-142">Folders</span><span class="sxs-lookup"><span data-stu-id="60ecd-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="60ecd-143">Folder</span><span class="sxs-lookup"><span data-stu-id="60ecd-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="60ecd-144">FolderId</span><span class="sxs-lookup"><span data-stu-id="60ecd-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="60ecd-145">Чтобы найти другие параметры для ответных сообщений операции CreateManagedFolder, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="60ecd-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="60ecd-146">Начните с элемента [креатеманажедфолдерреспонсе](createmanagedfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="60ecd-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="60ecd-147">Ответ об ошибке CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="60ecd-148">Description</span><span class="sxs-lookup"><span data-stu-id="60ecd-148">Description</span></span>

<span data-ttu-id="60ecd-149">В следующем примере кода показан ответ об ошибке для запроса CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="60ecd-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="60ecd-150">Код</span><span class="sxs-lookup"><span data-stu-id="60ecd-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="60ecd-151">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="60ecd-151">Error response elements</span></span>

<span data-ttu-id="60ecd-152">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="60ecd-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="60ecd-153">креатеманажедфолдерреспонсе</span><span class="sxs-lookup"><span data-stu-id="60ecd-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="60ecd-154">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="60ecd-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="60ecd-155">креатеманажедфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="60ecd-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="60ecd-156">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="60ecd-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="60ecd-157">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="60ecd-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="60ecd-158">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="60ecd-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="60ecd-159">Folders</span><span class="sxs-lookup"><span data-stu-id="60ecd-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="60ecd-160">См. также</span><span class="sxs-lookup"><span data-stu-id="60ecd-160">See also</span></span>



[<span data-ttu-id="60ecd-161">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-161">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="60ecd-162">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="60ecd-162">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="60ecd-163">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="60ecd-163">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="60ecd-164">Добавление управляемых папок</span><span class="sxs-lookup"><span data-stu-id="60ecd-164">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

