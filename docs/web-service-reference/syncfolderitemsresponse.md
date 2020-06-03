---
title: синкфолдеритемсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponse
api_type:
- schema
ms.assetid: 82fe0644-1756-40b2-955c-20c01110660c
description: Элемент Синкфолдеритемсреспонсе определяет ответ на запрос SyncFolderItems.
ms.openlocfilehash: 694730a5ead8b875da9b3544099d0b20a478a627
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530234"
---
# <a name="syncfolderitemsresponse"></a><span data-ttu-id="931e5-103">синкфолдеритемсреспонсе</span><span class="sxs-lookup"><span data-stu-id="931e5-103">SyncFolderItemsResponse</span></span>

<span data-ttu-id="931e5-104">Элемент **синкфолдеритемсреспонсе** определяет ответ на запрос SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="931e5-104">The **SyncFolderItemsResponse** element defines a response to a SyncFolderItems request.</span></span> 
  
```xml
<SyncFolderItemsResponse>
   <ResponseMessages/>
</SyncFolderItemsResponse>
```

 <span data-ttu-id="931e5-105">**синкфолдеритемсреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="931e5-105">**SyncFolderItemsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="931e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="931e5-106">Attributes and elements</span></span>

<span data-ttu-id="931e5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="931e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="931e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="931e5-108">Attributes</span></span>

<span data-ttu-id="931e5-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="931e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="931e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="931e5-110">Child elements</span></span>

|<span data-ttu-id="931e5-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="931e5-111">**Element**</span></span>|<span data-ttu-id="931e5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="931e5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="931e5-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="931e5-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="931e5-114">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="931e5-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="931e5-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="931e5-115">Parent elements</span></span>

<span data-ttu-id="931e5-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="931e5-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="931e5-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="931e5-117">Remarks</span></span>

<span data-ttu-id="931e5-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="931e5-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="931e5-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="931e5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="931e5-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="931e5-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="931e5-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="931e5-121">Schema name</span></span>  <br/> |<span data-ttu-id="931e5-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="931e5-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="931e5-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="931e5-123">Validation file</span></span>  <br/> |<span data-ttu-id="931e5-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="931e5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="931e5-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="931e5-125">Can be empty</span></span>  <br/> |<span data-ttu-id="931e5-126">False</span><span class="sxs-lookup"><span data-stu-id="931e5-126">False</span></span>  <br/> |
   

