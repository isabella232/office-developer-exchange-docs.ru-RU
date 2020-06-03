---
title: Работа с папками с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Узнайте, как создавать, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: a184d8da4d6949f01f47afc6a9fb7ed30729fd3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456383"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a><span data-ttu-id="e49d9-103">Работа с папками с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e49d9-103">Work with folders by using EWS in Exchange</span></span>

<span data-ttu-id="e49d9-104">Узнайте, как создавать, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e49d9-104">Learn how to create, get, update, and delete folders by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="e49d9-105">Для структурирования и упорядочивания почтовых ящиков в Exchange используются папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-105">EWS in Exchange uses folders to structure and organize mailboxes.</span></span> <span data-ttu-id="e49d9-106">Вы можете создавать новые, получать, обновлять и удалять папки с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-106">You can create new, get, update, and delete folders by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="e49d9-107">Каждый метод или операции, перечисленные в следующей таблице, выполняются для объекта [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) , типа [папки](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) или [одного из классов или типов производной папки](folders-and-items-in-ews-in-exchange.md#bk_folders).</span><span class="sxs-lookup"><span data-stu-id="e49d9-107">Each of the methods or operations listed in the following table is performed on a [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) object, a [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) type, or [one of the derived folder classes or types](folders-and-items-in-ews-in-exchange.md#bk_folders).</span></span>
  
<span data-ttu-id="e49d9-108">**Таблица 1. Методы и операции для создания, возврата, обновления и удаления папок**</span><span class="sxs-lookup"><span data-stu-id="e49d9-108">**Table 1. Methods and operations for creating, getting, updating and deleting folders**</span></span>

|<span data-ttu-id="e49d9-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="e49d9-109">**In order to…**</span></span>|<span data-ttu-id="e49d9-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="e49d9-110">**EWS Managed API method**</span></span>|<span data-ttu-id="e49d9-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="e49d9-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e49d9-112">Создание папки</span><span class="sxs-lookup"><span data-stu-id="e49d9-112">Create a folder</span></span>  <br/> |[<span data-ttu-id="e49d9-113">Folder. Save</span><span class="sxs-lookup"><span data-stu-id="e49d9-113">Folder.Save</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e49d9-114">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="e49d9-114">CreateFolder</span></span>](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e49d9-115">Создание иерархии папок</span><span class="sxs-lookup"><span data-stu-id="e49d9-115">Create a folder hierarchy</span></span>  <br/> |<span data-ttu-id="e49d9-116">Недоступно</span><span class="sxs-lookup"><span data-stu-id="e49d9-116">Not available</span></span>  <br/> |[<span data-ttu-id="e49d9-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="e49d9-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e49d9-118">Получение папки</span><span class="sxs-lookup"><span data-stu-id="e49d9-118">Get a folder</span></span>  <br/> |[<span data-ttu-id="e49d9-119">Folder. Bind</span><span class="sxs-lookup"><span data-stu-id="e49d9-119">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e49d9-120">GetFolder</span><span class="sxs-lookup"><span data-stu-id="e49d9-120">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e49d9-121">Получение иерархии папок</span><span class="sxs-lookup"><span data-stu-id="e49d9-121">Get a folder hierarchy</span></span>  <br/> |[<span data-ttu-id="e49d9-122">Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="e49d9-122">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e49d9-123">FindFolder</span><span class="sxs-lookup"><span data-stu-id="e49d9-123">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e49d9-124">Обновление папки</span><span class="sxs-lookup"><span data-stu-id="e49d9-124">Update a folder</span></span>  <br/> |[<span data-ttu-id="e49d9-125">Folder. Update</span><span class="sxs-lookup"><span data-stu-id="e49d9-125">Folder.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e49d9-126">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="e49d9-126">UpdateFolder</span></span>](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="e49d9-127">Удаление папки</span><span class="sxs-lookup"><span data-stu-id="e49d9-127">Delete a folder</span></span>  <br/> |[<span data-ttu-id="e49d9-128">Folder. Delete</span><span class="sxs-lookup"><span data-stu-id="e49d9-128">Folder.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="e49d9-129">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e49d9-129">DeleteFolder</span></span>](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<span data-ttu-id="e49d9-130"><a name="bk_createfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-130"><a name="bk_createfolderewsma"> </a></span></span>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="e49d9-131">Создание папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-131">Create a folder by using the EWS Managed API</span></span>

<span data-ttu-id="e49d9-132">В приведенном ниже примере кода показано, как использовать класс [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) для создания новой универсальной папки с [отображаемым именем](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) "Custom Folder" и значением свойства [фолдеркласс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) для платформы IPF. Ноте.</span><span class="sxs-lookup"><span data-stu-id="e49d9-132">The following code example shows how to use the [Folder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx) class to create a new generic folder with a [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) of "Custom Folder" and a [FolderClass](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx) property value of IPF.Note.</span></span> <span data-ttu-id="e49d9-133">Метод [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) сохраняет папку в качестве дочерней папки папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="e49d9-133">The [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method saves the folder as a child folder of the Inbox folder.</span></span> 
  
<span data-ttu-id="e49d9-134">В этих примерах предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e49d9-134">These examples assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="e49d9-135">Чтобы создать папку другого типа, например, [календарфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [контактсфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)или [тасксфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), создайте новый экземпляр определенного класса (вместо универсального класса **папки** ) и не задавайте свойство **фолдеркласс** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-135">To create a different type of folder, such as a [CalendarFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx), [ContactsFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx), [SearchFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx), or [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx), create a new instance of the specific class (instead of the generic **Folder** class) and do not set the **FolderClass** property.</span></span> <span data-ttu-id="e49d9-136">Например, в приведенном ниже примере кода показано, как создать новый объект [тасксфолдер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e49d9-136">For example, the following code example shows how to create a new [TasksFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx).</span></span>
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

<span data-ttu-id="e49d9-137">Если вы попытаетесь создать экземпляр определенного класса, а также задать свойство **фолдеркласс** , будет выдано сообщение об ошибке [еррорнофолдерклассоверриде](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-137">If you try to create an instance of a specific class and also set the **FolderClass** property, the [ErrorNoFolderClassOverride](https://msdn.microsoft.com/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx) error is thrown.</span></span> 
  
<span data-ttu-id="e49d9-138">Обратите внимание, что вы не можете пакетно создавать несколько папок в рамках одного вызова метода с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-138">Note that you cannot batch the creation of multiple folders in a single method call by using the EWS Managed API.</span></span>
  
## <a name="create-a-folder-by-using-ews"></a><span data-ttu-id="e49d9-139">Создание папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-139">Create a folder by using EWS</span></span>
<span data-ttu-id="e49d9-140"><a name="bk_createfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-140"><a name="bk_createfolderews"> </a></span></span>

<span data-ttu-id="e49d9-141">С помощью EWS можно создать одну папку или несколько папок.</span><span class="sxs-lookup"><span data-stu-id="e49d9-141">You can create a single folder or multiple of folders by using EWS.</span></span>
  
<span data-ttu-id="e49d9-142">Чтобы создать одну папку, отправьте сообщение запроса операции [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-142">To create a single folder, send a [CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) operation request message.</span></span> <span data-ttu-id="e49d9-143">Запрос операции **CreateFolder** указывает на то, что родительской папкой является папка "Входящие", [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) — "Custom Folder", а значение элемента [фолдеркласс](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) — IPF. Ноте.</span><span class="sxs-lookup"><span data-stu-id="e49d9-143">The **CreateFolder** operation request indicates that the parent folder is the Inbox, the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx) is "Custom Folder", and the [FolderClass](https://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx) element value is IPF.Note.</span></span> 
  
<span data-ttu-id="e49d9-144">Это также запрос XML, который управляемый API EWS отправляет, когда вы создаете новую папку и вызываете метод [Folder. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-144">This is also the XML request that the EWS Managed API sends when you create a new folder and call the [Folder.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e49d9-145">Сервер отвечает на запрос **CreateFolder** с сообщением [креатефолдерреспонсе](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **, указывающее, что**папка была успешно создана, и [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="e49d9-145">The server responds to the **CreateFolder** request with a [CreateFolderResponse](https://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder was created successfully, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="e49d9-146">Чтобы создать несколько папок, включите несколько элементов [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщение запроса операции **CreateFolder** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-146">To create multiple folders, include multiple [Folder](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **CreateFolder** operation request message.</span></span> <span data-ttu-id="e49d9-147">Все новые папки должны находиться в одной родительской папке.</span><span class="sxs-lookup"><span data-stu-id="e49d9-147">All the new folders must be in the same parent folder.</span></span> 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="e49d9-148">Создание иерархии папок с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-148">Create a folder hierarchy by using EWS</span></span>
<span data-ttu-id="e49d9-149"><a name="bk_createfolderhierarchy"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-149"><a name="bk_createfolderhierarchy"> </a></span></span>

<span data-ttu-id="e49d9-150">Вы можете создать иерархию папок в едином вызове с помощью операции [CREATEFOLDERPATH](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-150">You can create a folder hierarchy in a single call by using the EWS [CreateFolderPath](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="e49d9-151">Эта функция недоступна в управляемом API EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-151">The same functionality is not available in the EWS Managed API.</span></span> <span data-ttu-id="e49d9-152">Вместо этого, если вы используете управляемый API EWS, вы можете создавать папки по одному, как показано в разделе [Создание папки с помощью EWS](#bk_createfolderews).</span><span class="sxs-lookup"><span data-stu-id="e49d9-152">Instead, if you are using the EWS Managed API, you can create folders one by one, as shown in [Create a folder by using EWS](#bk_createfolderews).</span></span>
  
> [!NOTE]
> <span data-ttu-id="e49d9-153">Управляемый API EWS не реализует эту функцию.</span><span class="sxs-lookup"><span data-stu-id="e49d9-153">The EWS Managed API does not implement this functionality.</span></span> 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="e49d9-154">Получение папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-154">Get a folder by using the EWS Managed API</span></span>
<span data-ttu-id="e49d9-155"><a name="bk_getfolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-155"><a name="bk_getfolderewsma"> </a></span></span>

<span data-ttu-id="e49d9-156">В приведенном ниже примере кода показано, как использовать метод [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для получения папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="e49d9-156">The following code example shows how to use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to get the Inbox folder.</span></span> <span data-ttu-id="e49d9-157">Рекомендуется ограничить возвращаемые свойства только теми, которые необходимы для вашего приложения.</span><span class="sxs-lookup"><span data-stu-id="e49d9-157">As a best practice, limit the properties returned to only those required for your application.</span></span> <span data-ttu-id="e49d9-158">В этом примере показано, как ограничить возвращаемые свойства только свойством [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) , создав объект набор [свойств](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и применяя значение [идонли](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) к свойству [басепропертисет](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-158">This example limits the return properties to only include the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) property by creating a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) object and applying the [IdOnly](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx) value to the [BasePropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx) property.</span></span> 
  
<span data-ttu-id="e49d9-159">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="e49d9-159">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

<span data-ttu-id="e49d9-160">Если необходимо вернуть дополнительные свойства, добавьте свойства из класса [фолдерсчема](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) в набор **свойств**или используйте один из перегруженных методов [BIND](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , которые возвращают все свойства первого класса.</span><span class="sxs-lookup"><span data-stu-id="e49d9-160">If you need to return additional properties, add properties from the [FolderSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx) class to the **PropertySet**, or use one of the overloaded [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) methods that returns all first class properties.</span></span> 
  
<span data-ttu-id="e49d9-161">Обратите внимание, что вы не можете получить несколько папок одновременно с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-161">Note that you cannot get multiple folders at one time by using the EWS Managed API.</span></span> <span data-ttu-id="e49d9-162">Метод **BIND** необходимо вызывать отдельно для каждой папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-162">You have to call the **Bind** method on each folder separately.</span></span> 
  
## <a name="get-a-folder-by-using-ews"></a><span data-ttu-id="e49d9-163">Получение папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-163">Get a folder by using EWS</span></span>
<span data-ttu-id="e49d9-164"><a name="bk_getfolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-164"><a name="bk_getfolderews"> </a></span></span>

<span data-ttu-id="e49d9-165">С помощью EWS можно получить одну или несколько папок.</span><span class="sxs-lookup"><span data-stu-id="e49d9-165">You can get a single folder or multiple folders by using EWS.</span></span>
  
<span data-ttu-id="e49d9-166">Чтобы получить одну папку, отправьте серверу сообщение с запросом на выполнение операции с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-166">To get a single folder, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to the server.</span></span> <span data-ttu-id="e49d9-167">В следующем примере для параметра [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) задано значение **идонли**, поэтому возвращается только [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) указанной папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-167">In the following example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) is set to **IdOnly**, so only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the specified folder is returned.</span></span> <span data-ttu-id="e49d9-168">Элемент [фолдеридс](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) указывает, что извлекаемой папкой является папка "Входящие".</span><span class="sxs-lookup"><span data-stu-id="e49d9-168">The [FolderIds](https://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx) element indicates that the folder to retrieve is the Inbox folder.</span></span> 
  
<span data-ttu-id="e49d9-169">Это также запрос XML, который управляемый API EWS отправляет при выполнении связывания с папкой с помощью метода [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-169">This is also the XML request that the EWS Managed API sends when you bind to a folder by using the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="e49d9-170">Чтобы получить несколько папок, включите несколько элементов [фолдеридс](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) в сообщение с запросом операции "операция с **папкой** ".</span><span class="sxs-lookup"><span data-stu-id="e49d9-170">To get multiple folders, include multiple [FolderIds](https://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx) elements in the **GetFolder** operation request message.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e49d9-171">В следующем примере XML-кода показано сообщение [жетфолдерреспонсе](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции- **папки** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-171">The following XML example shows the [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) message that is sent from the server to the client in response to the **GetFolder** operation request.</span></span> <span data-ttu-id="e49d9-172">Он содержит только значение [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="e49d9-172">It only contains the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) value of the Inbox folder.</span></span> <span data-ttu-id="e49d9-173">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="e49d9-173">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a><span data-ttu-id="e49d9-174">Получение иерархии папок с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-174">Get a folder hierarchy by using the EWS Managed API</span></span>
<span data-ttu-id="e49d9-175"><a name="bk_getfolderhierarchyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-175"><a name="bk_getfolderhierarchyewsma"> </a></span></span>

<span data-ttu-id="e49d9-176">В приведенном ниже примере кода показано, как получить вложенные папки для указанной корневой папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-176">The following code example shows how to retrieve the subfolders for a specified root folder.</span></span> <span data-ttu-id="e49d9-177">В этом примере извлекаются подпапки папки **мсгфолдеррут** , которая является корнем поддерева IPM (где хранятся папки и элементы почтовых ящиков).</span><span class="sxs-lookup"><span data-stu-id="e49d9-177">This example retrieves the subfolders of the **MsgFolderRoot** folder, which is the root of the IPM Subtree (where your mailbox folders and items are stored).</span></span> 
  
<span data-ttu-id="e49d9-178">В этом примере создается объект класса [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) для ограничения результатов для ответа метода [Folder. финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-178">In this example, a [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class object is created to limit the results of the [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method response.</span></span> <span data-ttu-id="e49d9-179">В этом сценарии свойства возвращаются следующим образом: [ID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)и расширенное свойство, которое указывает, является ли эта папка скрытой.</span><span class="sxs-lookup"><span data-stu-id="e49d9-179">This scenario limits the properties to return to the following: [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx), [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx), and the extended property that indicates whether the folder is a hidden folder.</span></span> <span data-ttu-id="e49d9-180">Задайте для свойства [FolderView. обход](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) значение Deep, чтобы выполнить рекурсивный поиск, чтобы сервер возвращал подпапки, и присвойте корневому каталогу значение **мсгфолдеррут**, чтобы сервер возвращал все папки пользователя (а сервер не возвращал системные папки в поддереве без IPM).</span><span class="sxs-lookup"><span data-stu-id="e49d9-180">Set the [FolderView.Traversal](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx) value to Deep to perform a recursive search so that the server retrieves the subfolders, and set the root folder to **MsgFolderRoot**, so that the server returns all the user's folders (and the server does not return system folders in the Non-IPM Subtree).</span></span>
  
<span data-ttu-id="e49d9-181">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="e49d9-181">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="get-a-folder-hierarchy-by-using-ews"></a><span data-ttu-id="e49d9-182">Получение иерархии папок с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-182">Get a folder hierarchy by using EWS</span></span>
<span data-ttu-id="e49d9-183"><a name="bk_getfolderhierarchyews"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-183"><a name="bk_getfolderhierarchyews"> </a></span></span>

<span data-ttu-id="e49d9-184">В следующих примерах XML показано, как использовать операцию [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) для получения иерархии папок с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-184">The following XML examples show how to use the [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation to retrieve a folder hierarchy by using EWS.</span></span> <span data-ttu-id="e49d9-185">В этом примере показано получение папки **мсгфолдеррут** , которая является корнем поддерева IPM, и всех вложенных в нее папок.</span><span class="sxs-lookup"><span data-stu-id="e49d9-185">This example retrieves the **msgfolderroot** folder, which is the root of the IPM Subtree, and all its subfolders.</span></span> <span data-ttu-id="e49d9-186">Атрибуту **прохождения** присвоено значение **Deep** , чтобы сервер выполнял рекурсивный поиск в иерархии папок и возвращал только папки и вложенные папки в указанном корне в ответе.</span><span class="sxs-lookup"><span data-stu-id="e49d9-186">The **Traversal** attribute is set to **Deep** so that the server performs a recursive search of the folder hierarchy and only returns folders and subfolders under the specified root in the response.</span></span> <span data-ttu-id="e49d9-187">В этом примере элемент [басешапе](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) имеет значение **идонли** , чтобы сервер возвращал только элемент [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-187">In this example, the [BaseShape](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) element is set to **IdOnly** so that the server only returns the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="e49d9-188">Чтобы легче было понять выходные данные, включите элемент **DisplayName** в результаты, включив его в элемент [аддитионалпропертиес](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) в запросе вместе со значением **екстендедфиелдури** для свойства **PR_ATTR_HIDDEN** , чтобы узнать, являются ли папки скрытыми папками.</span><span class="sxs-lookup"><span data-stu-id="e49d9-188">To make the output easier to understand, include the **DisplayName** element in your results by including it in the [AdditionalProperties](https://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element in the request, along with the **ExtendedFieldURI** value for the **PR_ATTR_HIDDEN** property, so that you know whether the folders are hidden folders.</span></span> 
  
<span data-ttu-id="e49d9-189">Это также запрос XML, который управляемый API EWS отправляет при вызове метода [финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-189">This is also the XML request that the EWS Managed API sends when you call the [FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e49d9-190">В следующем примере XML-кода показано сообщение [финдфолдерреспонсе](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-190">The following XML example shows the [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that is sent from the server to the client in response to the **FindFolder** operation request.</span></span> <span data-ttu-id="e49d9-191">Он содержит только [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)и значение расширенного свойства **PR_ATTR_HIDDEN** для всех вложенных папок в папке **мсгрутфолдер** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-191">It contains only the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx), the [DisplayName](https://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx), and the value of the **PR_ATTR_HIDDEN** extended property for all the subfolders under the **msgrootfolder** folder.</span></span> <span data-ttu-id="e49d9-192">Если для элемента [value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) задано значение true, папка должна быть скрыта в клиентском представлении.</span><span class="sxs-lookup"><span data-stu-id="e49d9-192">If the [Value](https://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx) element is set to true, the folder should be hidden in the client view.</span></span> 
  
<span data-ttu-id="e49d9-193">Кроме того, это XML-ответ, который управляемый API EWS отправляет при получении нескольких папок с помощью метода [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-193">This is also the XML response that the EWS Managed API sends when you get multiple folders by using the [FindFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="e49d9-194">Значения некоторых атрибутов и элементов были сокращены для удобочитаемости, а некоторые папки не были включены для краткости.</span><span class="sxs-lookup"><span data-stu-id="e49d9-194">The values of some attributes and elements have been shortened for readability, and some folders have not been included for brevity.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="update-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="e49d9-195">Обновление папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-195">Update a folder by using the EWS Managed API</span></span>
<span data-ttu-id="e49d9-196"><a name="bk_updatefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-196"><a name="bk_updatefolderewsma"> </a></span></span>

<span data-ttu-id="e49d9-197">В приведенном ниже примере кода показано, как обновить отображаемое имя папки с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-197">The following code example shows how to update the display name of a folder by using the EWS Managed API.</span></span>
  
<span data-ttu-id="e49d9-198">Сначала создайте набор [свойств](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы ограничить число свойств, возвращаемых сервером в ответе [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-198">First, create a [PropertySet](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to limit the number of properties that the server returns in the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) response.</span></span> <span data-ttu-id="e49d9-199">Рекомендуется использовать **Басепропертисет** **идонли** для уменьшения числа вызовов к базе данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="e49d9-199">We recommend that you use the **IdOnly** **BasePropertySet** to reduce calls to the Exchange database.</span></span> <span data-ttu-id="e49d9-200">Затем используйте метод **BIND** для связывания с папкой, которую требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="e49d9-200">Next, use the **Bind** method to bind to the folder to update.</span></span> <span data-ttu-id="e49d9-201">Затем обновите свойство [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) и используйте метод [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) , чтобы сохранить изменения.</span><span class="sxs-lookup"><span data-stu-id="e49d9-201">Then, update the [DisplayName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx) property, and use the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
  
<span data-ttu-id="e49d9-202">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e49d9-202">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="e49d9-203">Локальная переменная *FolderId* — это [идентификатор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) обновляемой папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-203">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to update.</span></span> 
  
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

## <a name="update-a-folder-by-using-ews"></a><span data-ttu-id="e49d9-204">Обновление папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-204">Update a folder by using EWS</span></span>
<span data-ttu-id="e49d9-205"><a name="bk_updatefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-205"><a name="bk_updatefolderews"> </a></span></span>

<span data-ttu-id="e49d9-206">В приведенных ниже примерах XML-кода показано, как обновить отображаемое имя папки с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-206">The following XML examples show how to update the display name of a folder by using EWS.</span></span>
  
<span data-ttu-id="e49d9-207">Сначала отправьте сообщение с запросом на выполнение операции с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) , чтобы получить обновляемую папку, как показано в разделе [получение иерархии папок с помощью EWS](#bk_getfolderhierarchyews).</span><span class="sxs-lookup"><span data-stu-id="e49d9-207">First, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update, as shown in [Get a folder hierarchy by using EWS](#bk_getfolderhierarchyews).</span></span>
  
<span data-ttu-id="e49d9-208">Затем отправьте серверу сообщение с запросом на выполнение операции [операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) , чтобы обновить папку.</span><span class="sxs-lookup"><span data-stu-id="e49d9-208">Next, send an [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) operation request message to the server to update a folder.</span></span> <span data-ttu-id="e49d9-209">Запрос операции **операцию UpdateFolder** обновляет [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) на "обновленную настраиваемую папку".</span><span class="sxs-lookup"><span data-stu-id="e49d9-209">The **UpdateFolder** operation request updates the [DisplayName](https://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) to "Updated Custom Folder".</span></span> 
  
<span data-ttu-id="e49d9-210">Это также запрос XML, который отправляет управляемый API EWS при обновлении папки с помощью метода [Folder. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-210">This is also the XML request that the EWS Managed API sends when you update a folder by using the [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="e49d9-211">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="e49d9-211">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e49d9-212">Сервер отвечает на запрос **операцию UpdateFolder** с сообщением [упдатефолдерреспонсе](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, и [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки, которая была обновлена с помощью обновленного значения атрибута **чанжекэй** .</span><span class="sxs-lookup"><span data-stu-id="e49d9-212">The server responds to the **UpdateFolder** request with a [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, and the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder that was updated with an updated **ChangeKey** attribute value.</span></span> 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a><span data-ttu-id="e49d9-213">Удаление папки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-213">Delete a folder by using the EWS Managed API</span></span>
<span data-ttu-id="e49d9-214"><a name="bk_deletefolderewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-214"><a name="bk_deletefolderewsma"> </a></span></span>

<span data-ttu-id="e49d9-215">В этой статье представлен простой пример, в котором показано, как удалить папку с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-215">This article provides a basic example that shows you how to delete a folder by using the EWS Managed API.</span></span> <span data-ttu-id="e49d9-216">Более подробную информацию об удалении папок [можно узнать в статье Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="e49d9-216">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="e49d9-217">Чтобы удалить папку с помощью управляемого API EWS, сначала используйте метод [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) для связывания с объектом службы с удаляемой папкой.</span><span class="sxs-lookup"><span data-stu-id="e49d9-217">To delete a folder by using the EWS Managed API, first, use the [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) method to bind to the service object to the folder to delete.</span></span> <span data-ttu-id="e49d9-218">Затем используйте метод [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) для удаления папки с помощью режима удаления [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-218">Next, use the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method to delete the folder by using the [HardDelete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx) deletion mode.</span></span> 
  
<span data-ttu-id="e49d9-219">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="e49d9-219">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="e49d9-220">Локальная переменная *FolderId* — [идентификатор](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) удаляемой папки.</span><span class="sxs-lookup"><span data-stu-id="e49d9-220">The local variable  *folderId*  is the [Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) of the folder to delete.</span></span> 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a><span data-ttu-id="e49d9-221">Удаление папки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e49d9-221">Delete a folder by using EWS</span></span>
<span data-ttu-id="e49d9-222"><a name="bk_deletefolderews"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-222"><a name="bk_deletefolderews"> </a></span></span>

<span data-ttu-id="e49d9-223">В этой статье представлен базовый пример кода XML, в котором показано, как удалить папку с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="e49d9-223">This article provides a basic XML example that shows you how to delete a folder by using EWS.</span></span> <span data-ttu-id="e49d9-224">Более подробную информацию об удалении папок [можно узнать в статье Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="e49d9-224">For more details about deleting folders, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="e49d9-225">Чтобы удалить папку с помощью EWS, сначала отправьте сообщение с запросом операции "операция с [папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) ", чтобы получить обновляемую папку, как показано в разделе [Получение папки с помощью EWS](#bk_getfolderews).</span><span class="sxs-lookup"><span data-stu-id="e49d9-225">To delete a folder by using EWS, first, send a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) operation request message to get the folder to update as shown in [Get a folder by using EWS](#bk_getfolderews).</span></span> 
  
<span data-ttu-id="e49d9-226">Затем отправьте серверу запрос на получение сообщения об операции [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) , чтобы удалить папку.</span><span class="sxs-lookup"><span data-stu-id="e49d9-226">Next, send a [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) operation request message to the server to delete the folder.</span></span> <span data-ttu-id="e49d9-227">Запрос операции **DeleteFolder** указывает на то, что **делететипе** является **HardDelete** и включает [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) папки для удаления.</span><span class="sxs-lookup"><span data-stu-id="e49d9-227">The **DeleteFolder** operation request indicates that the **DeleteType** is **HardDelete** and it includes the [FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) of the folder to delete.</span></span> 
  
<span data-ttu-id="e49d9-228">Это также запрос XML, который отправляет управляемый API EWS при удалении папки с помощью метода [Folder. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e49d9-228">This is also the XML request that the EWS Managed API sends when you delete a folder by using the [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="e49d9-229">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="e49d9-229">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e49d9-230">Сервер отвечает на запрос **DeleteFolder** с сообщением [делетефолдерреспонсе](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, что указывает на то, что удаление папки прошло успешно.</span><span class="sxs-lookup"><span data-stu-id="e49d9-230">The server responds to the **DeleteFolder** request with a [DeleteFolderResponse](https://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx) message that includes the a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the folder deletion was successful.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="e49d9-231">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="e49d9-231">Next steps</span></span>
<span data-ttu-id="e49d9-232"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="e49d9-232"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="e49d9-233">После получения папок на сервере или внесения изменений в папки может потребоваться [Синхронизация иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [Подписка на уведомления об изменениях папки](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) на сервере.</span><span class="sxs-lookup"><span data-stu-id="e49d9-233">After you have retrieved the folders on the server, or made changes to folders, you might want to [synchronize your folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [subscribe to notifications about folder changes](notification-subscriptions-mailbox-events-and-ews-in-exchange.md) on the server.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e49d9-234">См. также</span><span class="sxs-lookup"><span data-stu-id="e49d9-234">See also</span></span>

- [<span data-ttu-id="e49d9-235">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="e49d9-235">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)   
- [<span data-ttu-id="e49d9-236">Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e49d9-236">Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="e49d9-237">Удаление элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e49d9-237">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)   
- [<span data-ttu-id="e49d9-238">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="e49d9-238">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    

