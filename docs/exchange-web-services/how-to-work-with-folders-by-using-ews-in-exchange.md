---
title: Работа с папками с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Узнайте, как создание, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761149"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="da734-103">Работа с папками с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="da734-104">Узнайте, как создание, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="da734-105">ВЕБ-службах Exchange использует папки для структурирования и организации почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="da734-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="da734-106">Можно создать новый, получение, обновление и удаление папок с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="da734-107">Каждый из методов или операции, перечисленные в следующей таблице выполняется на объект [Folder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , типа [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) или [один из папки производные классы или типы](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="da734-107">Each of the methods or operations listed in the following table is performed on a [Folder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="da734-108">**В таблице 1. Методы и операции создание, получение, обновление и удаление папок**</span><span class="sxs-lookup"><span data-stu-id="da734-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="da734-109">**Чтобы...**</span><span class="sxs-lookup"><span data-stu-id="da734-109">**In order to…**</span></span>|<span data-ttu-id="da734-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="da734-110">**EWS Managed API method**</span></span>|<span data-ttu-id="da734-111">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="da734-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="da734-112">Создайте папку</span><span class="sxs-lookup"><span data-stu-id="da734-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="da734-113">Folder.Save</span><span class="sxs-lookup"><span data-stu-id="da734-113">Folder.Save</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="da734-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="da734-114">CreateFolder</span></span>](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="da734-115">Создание иерархии папок</span><span class="sxs-lookup"><span data-stu-id="da734-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="da734-116">Недоступна</span><span class="sxs-lookup"><span data-stu-id="da734-116">Not available</span></span>  <br/> |[<span data-ttu-id="da734-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="da734-117">CreateFolderPath</span></span>](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="da734-118">Получение папки</span><span class="sxs-lookup"><span data-stu-id="da734-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="da734-119">Folder.Bind</span><span class="sxs-lookup"><span data-stu-id="da734-119">Folder.Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="da734-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="da734-120">GetFolder</span></span>](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="da734-121">Получение иерархии папок</span><span class="sxs-lookup"><span data-stu-id="da734-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="da734-122">Folder.FindFolders</span><span class="sxs-lookup"><span data-stu-id="da734-122">Folder.FindFolders</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="da734-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="da734-123">FindFolder</span></span>](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="da734-124">Изменение папки</span><span class="sxs-lookup"><span data-stu-id="da734-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="da734-125">Folder.Update</span><span class="sxs-lookup"><span data-stu-id="da734-125">Folder.Update</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="da734-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="da734-126">UpdateFolder</span></span>](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="da734-127">Удаление папки</span><span class="sxs-lookup"><span data-stu-id="da734-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="da734-128">Folder.Delete</span><span class="sxs-lookup"><span data-stu-id="da734-128">Folder.Delete</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="da734-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="da734-129">DeleteFolder</span></span>](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="da734-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-130"></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="da734-131">Создайте папку с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="da734-132">В следующем примере кода показано, как использовать класс [папку](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) для создания новой общей папки с [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) «Настраиваемые папки» и значение свойства [FolderClass](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) IPF. Примечание.</span><span class="sxs-lookup"><span data-stu-id="da734-132">The following code example shows how to use the [Folder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="da734-133">Метод [Folder.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) сохраняет папку в качестве дочерней папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="da734-133">The [Folder.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="da734-134">В этих примерах предполагается этой **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-134">These examples assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="da734-135">Для создания другого типа папки, например [CalendarFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)или [TasksFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), создайте новый экземпляр объекта определенного класса (а не универсальный класс **папки** ) и не задана Свойство **FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="da734-135">To create a different type of folder, such as a [CalendarFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="da734-136">Например в следующем примере кода показано, как создать новый [TasksFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="da734-136">For example, the following code example shows how to create a new [TasksFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="da734-137">При попытке создать экземпляр определенного класса, а также необходимо задать свойство **FolderClass** , возникает ошибка [ErrorNoFolderClassOverride](http://msdn.microsoft.com/ru-ru/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](http://msdn.microsoft.com/ru-ru/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="da734-138">Обратите внимание, что нельзя Пакетное создание несколько папок в одном методе с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="da734-139">Создайте папку с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-139">Create a folder by using EWS</span></span>
<span data-ttu-id="da734-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-140"></span></span>

<span data-ttu-id="da734-141">Можно создать несколько папок или одной папке с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="da734-142">Для создания единого папки, отправьте сообщение [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) операции запроса.</span><span class="sxs-lookup"><span data-stu-id="da734-142">To create a single folder, send a [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="da734-143">Запрос операции **CreateFolder** указывает, что родительской папки — это папки «Входящие», [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) — это «Настраиваемая папка» и значения элемента [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) является IPF. Примечание.</span><span class="sxs-lookup"><span data-stu-id="da734-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="da734-144">Это также XML-запрос, который отправляет управляемый API EWS при создании новой папки и вызовите метод [Folder.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="da734-145">Сервер отвечает на запрос **CreateFolder** [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что папка была создана успешно, и [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) из только что созданный сообщение.</span><span class="sxs-lookup"><span data-stu-id="da734-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="da734-146">Чтобы создать несколько папок, включают несколько элементов [папки](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщении **CreateFolder** операции запроса.</span><span class="sxs-lookup"><span data-stu-id="da734-146">To create multiple folders, include multiple [Folder](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="da734-147">Все новые папки должен быть в одной родительской папке.</span><span class="sxs-lookup"><span data-stu-id="da734-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="da734-148">Создание иерархии папок с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="da734-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-149"></span></span>

<span data-ttu-id="da734-150">Можно создать иерархии папок в одном вызове с помощью операции EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="da734-151">Те же функциональные возможности недоступен в управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="da734-152">Вместо этого при использовании управляемого интерфейса API веб-служб Exchange, можно создавать папки по одному, как показано в разделе [Создание папки с помощью веб-служб Exchange](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="da734-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="da734-153">Управляемый API EWS не реализует эту функцию.</span><span class="sxs-lookup"><span data-stu-id="da734-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="da734-154">Получение папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="da734-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-155"></span></span>

<span data-ttu-id="da734-156">В следующем примере кода показано, как использовать метод [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для получения папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="da734-156">The following code example shows how to use the [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="da734-157">Рекомендуется ограничивайте возвращаемые только теми, необходимый для приложения свойства.</span><span class="sxs-lookup"><span data-stu-id="da734-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="da734-158">В этом примере ограничивается возвращаемого свойства можно включить только свойство [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , создав объект [PropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и применения [IdOnly](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) значения для свойства [BasePropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-158">This example limits the return properties to only include the [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="da734-159">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-159">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="da734-160">Если вам потребуется получить дополнительные свойства, добавьте свойства из класса [FolderSchema](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) **PropertySet**или использовать один из перегруженных методов [привязки](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , которые возвращаются все свойства первого класса.</span><span class="sxs-lookup"><span data-stu-id="da734-160">If you need to return additional properties, add properties from the [FolderSchema](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="da734-161">Следует отметить, что нельзя одновременно несколько папок с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="da734-162">Необходимо вызвать метод **привязки** для каждой папки отдельно.</span><span class="sxs-lookup"><span data-stu-id="da734-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="da734-163">Получение папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-163">Get a folder by using EWS</span></span>
<span data-ttu-id="da734-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-164"></span></span>

<span data-ttu-id="da734-165">Можно получить одной папке или несколько папок с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="da734-166">Для получения одной папке отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса к серверу.</span><span class="sxs-lookup"><span data-stu-id="da734-166">To get a single folder, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="da734-167">В следующем примере устанавливается [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) для **IdOnly**, возвращается только [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) указанной папки.</span><span class="sxs-lookup"><span data-stu-id="da734-167">In the following example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="da734-168">Элемент [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) указывает, что папка для извлечения папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="da734-168">The [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="da734-169">Это также XML-запрос, который отправляет управляемый API EWS при связывании в папку с помощью метода [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="da734-170">Чтобы получить несколько папок, включают несколько элементов [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщении **GetFolder** операции запроса.</span><span class="sxs-lookup"><span data-stu-id="da734-170">To get multiple folders, include multiple [FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="da734-171">В следующем примере XML показано [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) сообщение, которое отправляется с сервера на клиент в ответ на запрос операции **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="da734-171">The following XML example shows the [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="da734-172">Содержит только значение [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="da734-172">It only contains the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="da734-173">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="da734-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="da734-174">Получение иерархии папок с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="da734-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-175"></span></span>

<span data-ttu-id="da734-176">В следующем примере кода показано, как получить вложенные папки для указанной корневой папке.</span><span class="sxs-lookup"><span data-stu-id="da734-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="da734-177">В этом примере показано получение вложенные папки в папку **MsgFolderRoot** , которая является корневым каталогом поддерева IPM (папки почтовых ящиков и элементы хранения).</span><span class="sxs-lookup"><span data-stu-id="da734-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="da734-178">В этом примере объект класса [FolderView](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) создается для ограничения результатов ответа метода [Folder.FindFolders](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-178">In this example, a [FolderView](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="da734-179">Этот сценарий ограничивает возвращаемых для следующих свойств: [идентификатор](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)и расширенные свойства, которое указывает, является ли папка является скрытым.</span><span class="sxs-lookup"><span data-stu-id="da734-179">This scenario limits the properties to return to the following: [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="da734-180">Задайте значение [FolderView.Traversal](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) глубокое для выполнения рекурсивный поиск, чтобы сервер получает вложенных папок, а значение в корневой папке **MsgFolderRoot**, чтобы сервер возвращает все папках пользователя (и сервер не возвращает системные папки поддерева IPM не).</span><span class="sxs-lookup"><span data-stu-id="da734-180">Set the [FolderView.Traversal](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="da734-181">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-181">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="da734-182">Получение иерархии папок с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="da734-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-183"></span></span>

<span data-ttu-id="da734-184">В следующих примерах XML для получения иерархии папок с помощью веб-служб Exchange с помощью операции [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-184">The following XML examples show how to use the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="da734-185">В этом примере извлекается в папку **msgfolderroot** , которая является корневым каталогом поддерева IPM и все вложенные папки.</span><span class="sxs-lookup"><span data-stu-id="da734-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="da734-186">Атрибут **обхода** присваивается **глубокое** , чтобы сервер выполняет рекурсивный поиск в иерархии папок и возвращает только папки и вложенные папки в корневом каталоге указанного в ответе.</span><span class="sxs-lookup"><span data-stu-id="da734-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="da734-187">В следующем примере элемент [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) присваивается **IdOnly** , чтобы сервер только возвращает элемент [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-187">In this example, the [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="da734-188">Чтобы облегчить понимание выходные данные, включите элемент **DisplayName** в результатах, включив в элемент [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) в запросе, а также значение **ExtendedFieldURI** для **PR_ATTR_HIDDEN** свойства, чтобы знать, являются ли папки скрытые папки.</span><span class="sxs-lookup"><span data-stu-id="da734-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="da734-189">Это также запроса XML, то при вызове метода [FindFolders](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) отправляет управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="da734-190">В следующем примере XML показано [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) сообщение, которое отправляется с сервера на клиент в ответ на запрос операции **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="da734-190">The following XML example shows the [FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="da734-191">Он содержит только [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), и значение **PR_ATTR_HIDDEN** расширенные свойства для всех вложенных папок в папке **msgrootfolder** .</span><span class="sxs-lookup"><span data-stu-id="da734-191">It contains only the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="da734-192">Если [значение](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) элемента задано значение true, папка должны быть скрыты в представлении клиента.</span><span class="sxs-lookup"><span data-stu-id="da734-192">If the [Value](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="da734-193">Это также XML-ответ, который отправляет управляемый API веб-служб Exchange, когда вы получаете несколько папок с помощью метода [FindFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="da734-194">Значения некоторые атрибуты и элементы URL были сокращены для удобства чтения и некоторые папки не были включены для краткости.</span><span class="sxs-lookup"><span data-stu-id="da734-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="da734-195">Изменение папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="da734-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-196"></span></span>

<span data-ttu-id="da734-197">В следующем примере кода показано, как обновить отображаемое имя папки с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="da734-198">Во-первых создайте [PropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы ограничить число свойств, которые сервер возвращает в ответе [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-198">First, create a [PropertySet](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="da734-199">Мы рекомендуем использовать **IdOnly** **BasePropertySet** для уменьшения обращений к базе данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="da734-200">Затем используйте метод **Bind** для привязки к папке требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="da734-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="da734-201">Затем обновите свойство [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) и используйте метод [Folder.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="da734-201">Then, update the [DisplayName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="da734-202">В этом примере мы предполагаем этой **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-202">In this example, we assume that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="da734-203">Локальной переменной *folderId* — это [идентификатор](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) папки для обновления.</span><span class="sxs-lookup"><span data-stu-id="da734-203">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="da734-204">Изменение папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-204">Update a folder by using EWS</span></span>
<span data-ttu-id="da734-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-205"></span></span>

<span data-ttu-id="da734-206">В следующих примерах XML показано, как обновить отображаемое имя папки с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="da734-207">Во-первых отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса на получение папки для обновления, как показано в [Начало иерархии папок с помощью веб-служб Exchange](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="da734-207">First, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="da734-208">Затем отправьте сообщение [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) операция запроса сервером, чтобы обновить папку.</span><span class="sxs-lookup"><span data-stu-id="da734-208">Next, send an [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="da734-209">Запрос операции **UpdateFolder** обновляет [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) «Обновить папку Custom».</span><span class="sxs-lookup"><span data-stu-id="da734-209">The **UpdateFolder** operation request updates the [DisplayName](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="da734-210">Это также XML-запрос, который отправляет управляемый API EWS при обновлении папки с помощью метода [Folder.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="da734-211">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="da734-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="da734-212">Сервер отвечает на запрос **UpdateFolder** [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) **NoError**и [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки, которая была обновлена с обновленные ** ChangeKey** значение атрибута.</span><span class="sxs-lookup"><span data-stu-id="da734-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="da734-213">Удаление папки с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="da734-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-214"></span></span>

<span data-ttu-id="da734-215">В этой статье приводятся основные пример, в котором показано, как удалить папку с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="da734-216">Для получения дополнительных сведений об удалении папок видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="da734-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="da734-217">Чтобы удалить папку с помощью управляемого интерфейса API веб-служб Exchange, во-первых, используйте метод [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для привязки к объекту службы в папку для удаления.</span><span class="sxs-lookup"><span data-stu-id="da734-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="da734-218">Затем используйте метод [Folder.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) удалить папку с помощью режима удаления [HardDelete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-218">Next, use the [Folder.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="da734-219">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-219">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="da734-220">Локальной переменной *folderId* — это [идентификатор](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) папки для удаления.</span><span class="sxs-lookup"><span data-stu-id="da734-220">The local variable  *folderId*  is the [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="da734-221">Удаление папки с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="da734-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-222"></span></span>

<span data-ttu-id="da734-223">В этой статье приводятся основные примере XML-кода показано, как удалить папку с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="da734-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="da734-224">Для получения дополнительных сведений об удалении папок видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="da734-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="da734-225">Удалить папку с помощью веб-служб Exchange, во-первых, отправьте сообщение [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) операция запроса на получение папки для обновления, как показано на [Получение папки с помощью веб-служб Exchange](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="da734-225">To delete a folder by using EWS, first, send a [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="da734-226">Далее отправьте сообщение [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) операция запроса сервером, чтобы удалить папку.</span><span class="sxs-lookup"><span data-stu-id="da734-226">Next, send a [DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="da734-227">Запрос операции **DeleteFolder** указывает, что **DeleteType** **HardDelete** и включает [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки для удаления.</span><span class="sxs-lookup"><span data-stu-id="da734-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="da734-228">Это также XML-запрос, который отправляет управляемый API EWS при удалении папки с помощью метода [Folder.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="da734-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="da734-229">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="da734-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="da734-230">Сервер отвечает на запрос **DeleteFolder** [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что удаление папки прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="da734-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/ru-ru/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="da734-231">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="da734-231">Next steps</span></span>
<span data-ttu-id="da734-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="da734-232"></span></span>

<span data-ttu-id="da734-233">После извлечения папок на сервере, или внесенные изменения к папкам, может потребоваться [Синхронизация иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [подписаться на уведомления об изменениях в папку](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) на сервере.</span><span class="sxs-lookup"><span data-stu-id="da734-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="da734-234">См. также</span><span class="sxs-lookup"><span data-stu-id="da734-234">See also</span></span>

- [<span data-ttu-id="da734-235">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="da734-236">Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="da734-237">Удаление элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="da734-238">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="da734-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

