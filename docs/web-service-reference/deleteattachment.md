---
title: DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 43d0c1cb-92ca-4399-9b3a-acb2b5c22624
description: Элемент DeleteAttachment является корневым элементом в запросе на удаление вложения из хранилища Exchange.
ms.openlocfilehash: 2beedd647febf025f6e3140ec37b196c9aeb7611
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762018"
---
# <a name="deleteattachment"></a><span data-ttu-id="68058-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="68058-103">DeleteAttachment</span></span>

<span data-ttu-id="68058-104">Элемент **DeleteAttachment** является корневым элементом в запросе на удаление вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="68058-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="68058-105">**DeleteAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="68058-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="68058-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="68058-106">Attributes and elements</span></span>

<span data-ttu-id="68058-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="68058-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="68058-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="68058-108">Attributes</span></span>

<span data-ttu-id="68058-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="68058-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="68058-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="68058-110">Child elements</span></span>

|<span data-ttu-id="68058-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="68058-111">**Element**</span></span>|<span data-ttu-id="68058-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="68058-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="68058-113">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="68058-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="68058-114">Содержит массив идентификаторов вложения, которые используются для удаления вложения.</span><span class="sxs-lookup"><span data-stu-id="68058-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="68058-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="68058-115">Parent elements</span></span>

<span data-ttu-id="68058-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="68058-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="68058-117">Замечания</span><span class="sxs-lookup"><span data-stu-id="68058-117">Remarks</span></span>

<span data-ttu-id="68058-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="68058-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="68058-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="68058-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="68058-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="68058-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="68058-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="68058-121">Schema Name</span></span>  <br/> |<span data-ttu-id="68058-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="68058-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="68058-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="68058-123">Validation File</span></span>  <br/> |<span data-ttu-id="68058-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="68058-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="68058-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="68058-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="68058-126">False</span><span class="sxs-lookup"><span data-stu-id="68058-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="68058-127">См. также</span><span class="sxs-lookup"><span data-stu-id="68058-127">See also</span></span>

- [<span data-ttu-id="68058-128">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="68058-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

