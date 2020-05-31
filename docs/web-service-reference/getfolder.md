---
title: GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 34e4c9ea-adcd-46bd-ae8f-7abb256c585a
description: Элемент Folder определяет запрос на получение папки из почтового ящика в хранилище Exchange.
ms.openlocfilehash: 233da6ce57683350d4a13f6585593ac09438f0e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762797"
---
# <a name="getfolder"></a><span data-ttu-id="7a6e8-103">GetFolder</span><span class="sxs-lookup"><span data-stu-id="7a6e8-103">GetFolder</span></span>

<span data-ttu-id="7a6e8-104">Элемент **Folder** определяет запрос на получение папки из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-104">The **GetFolder** element defines a request to get a folder from a mailbox in the Exchange store.</span></span> 
  
```xml
<GetFolder>
   <FolderShape/>
   <FolderIds/>
</GetFolder>
```

 <span data-ttu-id="7a6e8-105">**жетфолдертипе**</span><span class="sxs-lookup"><span data-stu-id="7a6e8-105">**GetFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a6e8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a6e8-106">Attributes and elements</span></span>

<span data-ttu-id="7a6e8-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a6e8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a6e8-108">Attributes</span></span>

<span data-ttu-id="7a6e8-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a6e8-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a6e8-110">Child elements</span></span>

|<span data-ttu-id="7a6e8-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a6e8-111">**Element**</span></span>|<span data-ttu-id="7a6e8-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a6e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a6e8-113">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="7a6e8-113">FolderShape</span></span>](foldershape.md) <br/> |<span data-ttu-id="7a6e8-114">Определяет свойства, которые необходимо получить для каждой папки, указанной в элементе [фолдеридс](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="7a6e8-114">Identifies the properties to get for each folder identified in the [FolderIds](folderids.md) element.</span></span>  <br/> |
|[<span data-ttu-id="7a6e8-115">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="7a6e8-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="7a6e8-116">Содержит массив идентификаторов папок, которые используются для идентификации папок, получаемых из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-116">Contains an array of folder identifiers that are used to identify folders to get from a mailbox in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a6e8-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a6e8-117">Parent elements</span></span>

<span data-ttu-id="7a6e8-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7a6e8-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="7a6e8-119">Remarks</span></span>

<span data-ttu-id="7a6e8-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7a6e8-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a6e8-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a6e8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a6e8-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a6e8-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a6e8-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a6e8-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7a6e8-124">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="7a6e8-124">Message schema</span></span>  <br/> |
|<span data-ttu-id="7a6e8-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a6e8-125">Validation File</span></span>  <br/> |<span data-ttu-id="7a6e8-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7a6e8-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a6e8-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a6e8-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a6e8-128">False</span><span class="sxs-lookup"><span data-stu-id="7a6e8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a6e8-129">См. также</span><span class="sxs-lookup"><span data-stu-id="7a6e8-129">See also</span></span>



[<span data-ttu-id="7a6e8-130">Операция GetFolder</span><span class="sxs-lookup"><span data-stu-id="7a6e8-130">GetFolder operation</span></span>](getfolder-operation.md)

