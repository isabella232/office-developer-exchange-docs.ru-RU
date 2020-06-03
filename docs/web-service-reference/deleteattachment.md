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
ms.openlocfilehash: ae8dd5abc1dced2645e579a62f1f57a66cbc9877
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457349"
---
# <a name="deleteattachment"></a><span data-ttu-id="d5fe7-103">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d5fe7-103">DeleteAttachment</span></span>

<span data-ttu-id="d5fe7-104">Элемент **DeleteAttachment** является корневым элементом в запросе на удаление вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-104">The **DeleteAttachment** element is the root element in a request to delete an attachment from the Exchange store.</span></span> 
  
```xml
<DeleteAttachment>
   <AttachmentIds/>
</DeleteAttachment>
```

<span data-ttu-id="d5fe7-105">**делетеаттачменттипе**</span><span class="sxs-lookup"><span data-stu-id="d5fe7-105">**DeleteAttachmentType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d5fe7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d5fe7-106">Attributes and elements</span></span>

<span data-ttu-id="d5fe7-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5fe7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d5fe7-108">Attributes</span></span>

<span data-ttu-id="d5fe7-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5fe7-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d5fe7-110">Child elements</span></span>

|<span data-ttu-id="d5fe7-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d5fe7-111">**Element**</span></span>|<span data-ttu-id="d5fe7-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d5fe7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5fe7-113">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="d5fe7-113">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="d5fe7-114">Содержит массив идентификаторов вложений, которые используются для удаления вложений.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-114">Contains an array of attachment identifiers that are used to delete the attachments.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d5fe7-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d5fe7-115">Parent elements</span></span>

<span data-ttu-id="d5fe7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5fe7-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="d5fe7-117">Remarks</span></span>

<span data-ttu-id="d5fe7-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d5fe7-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5fe7-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d5fe7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5fe7-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d5fe7-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d5fe7-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d5fe7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d5fe7-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d5fe7-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d5fe7-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d5fe7-123">Validation File</span></span>  <br/> |<span data-ttu-id="d5fe7-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d5fe7-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d5fe7-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d5fe7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5fe7-126">False</span><span class="sxs-lookup"><span data-stu-id="d5fe7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5fe7-127">См. также</span><span class="sxs-lookup"><span data-stu-id="d5fe7-127">See also</span></span>

- [<span data-ttu-id="d5fe7-128">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="d5fe7-128">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

