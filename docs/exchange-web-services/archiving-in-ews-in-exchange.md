---
title: Архивация в веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 78ae179b-ae4f-4f64-911a-e0c70e0fa314
description: Сведения о том, как архивировать в EWS в Exchange.
ms.openlocfilehash: b433b9f88905ee255720e8b341d560fa0e464975
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456215"
---
# <a name="archiving-in-ews-in-exchange"></a><span data-ttu-id="52c50-103">Архивация в веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="52c50-103">Archiving in EWS in Exchange</span></span>

<span data-ttu-id="52c50-104">Сведения о том, как архивировать в EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="52c50-104">Learn about archiving in EWS in Exchange.</span></span>
  
<span data-ttu-id="52c50-105">Архивные почтовые ящики это дополнительные почтовые ящики, связанные с пользователем.</span><span class="sxs-lookup"><span data-stu-id="52c50-105">Archive mailboxes are secondary mailboxes that are associated with a user.</span></span> <span data-ttu-id="52c50-106">Архивные почтовые ящики обычно используются для управления пределами хранилища электронной почты.</span><span class="sxs-lookup"><span data-stu-id="52c50-106">Archive mailboxes are typically used to manage email storage limits.</span></span> <span data-ttu-id="52c50-107">Например, старые элементы электронной почты можно периодически перемещать из папки "Входящие" в архивный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="52c50-107">For example, older email items might periodically be moved from the Inbox to the archive mailbox.</span></span> 
  
<span data-ttu-id="52c50-108">Exchange Online, Exchange Online в составе Office 365, а Exchange Server 2013 — это две новые операции веб-служб Exchange (EWS), которые можно использовать для архивации набора почтовых элементов из основного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="52c50-108">Exchange Online, Exchange Online as part of Office 365, and Exchange Server 2013 introduce two new Exchange Web Services (EWS) operations that you can use to archive a set of mail items from a primary mailbox.</span></span> <span data-ttu-id="52c50-109">Архивирование элементов папки "Входящие" таким способом сохраняет иерархию папок для элементов.</span><span class="sxs-lookup"><span data-stu-id="52c50-109">Archiving Inbox items in this way preserves the folder hierarchy of the items.</span></span> <span data-ttu-id="52c50-110">Кроме того, архивные почтовые ящики теперь можно хранить локально на клиенте или удаленно, как правило, как правило, непрозрачным для пользователя, используя путь к папке для ссылки на содержимое архива.</span><span class="sxs-lookup"><span data-stu-id="52c50-110">In addition, archive mailboxes can now be stored either locally on a client, or remotely, in a way that is mostly opaque to a user, by using a folder path to point to the contents of the archive.</span></span>
  
## <a name="archiving-operations-in-ews"></a><span data-ttu-id="52c50-111">Операции архивирования в EWS</span><span class="sxs-lookup"><span data-stu-id="52c50-111">Archiving operations in EWS</span></span>

<span data-ttu-id="52c50-112">В следующей таблице перечислены операции архивирования, которые были представлены в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="52c50-112">The following table lists the archiving operations that were introduced in Exchange 2013.</span></span> 
  
|<span data-ttu-id="52c50-113">**Имя операции**</span><span class="sxs-lookup"><span data-stu-id="52c50-113">**Operation name**</span></span>|<span data-ttu-id="52c50-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="52c50-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="52c50-115">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="52c50-115">ArchiveItem</span></span>](https://msdn.microsoft.com/library/1af216b3-13ea-498e-b4fc-23513755d731%28Office.15%29.aspx) <br/> |<span data-ttu-id="52c50-116">Перемещает элемент из основного почтового ящика в архивный.</span><span class="sxs-lookup"><span data-stu-id="52c50-116">Moves an item from the primary mailbox to the archive mailbox.</span></span>  <br/> |
|[<span data-ttu-id="52c50-117">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="52c50-117">CreateFolderPath</span></span>](https://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |<span data-ttu-id="52c50-118">Создает URI, указывающий на место хранения архивного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="52c50-118">Creates a URI that points to the storage location for the archive mailbox.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="52c50-119">См. также</span><span class="sxs-lookup"><span data-stu-id="52c50-119">See also</span></span>

- [<span data-ttu-id="52c50-120">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="52c50-120">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)
    
- [<span data-ttu-id="52c50-121">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="52c50-121">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)
    
- [<span data-ttu-id="52c50-122">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="52c50-122">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    

