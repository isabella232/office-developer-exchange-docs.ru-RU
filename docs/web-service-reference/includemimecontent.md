---
title: инклудемимеконтент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: Элемент Инклудемимеконтент указывает, будет ли в ответе возвращаться содержимое MIME для элемента или вложения.
ms.openlocfilehash: 6198e4bef2dc59e6e56a8d3cbe463dad13e544e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457195"
---
# <a name="includemimecontent"></a><span data-ttu-id="85530-103">инклудемимеконтент</span><span class="sxs-lookup"><span data-stu-id="85530-103">IncludeMimeContent</span></span>

<span data-ttu-id="85530-104">Элемент **инклудемимеконтент** указывает, будет ли в ответе ВОЗВРАЩАТЬСЯ содержимое MIME для элемента или вложения.</span><span class="sxs-lookup"><span data-stu-id="85530-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="85530-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="85530-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85530-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="85530-106">Attributes and elements</span></span>

<span data-ttu-id="85530-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="85530-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85530-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="85530-108">Attributes</span></span>

<span data-ttu-id="85530-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85530-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85530-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="85530-110">Child elements</span></span>

<span data-ttu-id="85530-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="85530-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85530-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="85530-112">Parent elements</span></span>

|<span data-ttu-id="85530-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85530-113">**Element**</span></span>|<span data-ttu-id="85530-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85530-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85530-115">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="85530-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="85530-116">Определяет дополнительные свойства, возвращаемые в ответе на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="85530-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="85530-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="85530-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="85530-118">итемшапе</span><span class="sxs-lookup"><span data-stu-id="85530-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="85530-119">Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="85530-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="85530-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="85530-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85530-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="85530-121">Text value</span></span>

<span data-ttu-id="85530-122">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="85530-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="85530-123">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="85530-123">The default value is **false**.</span></span> <span data-ttu-id="85530-124">Это логический тип данных.</span><span class="sxs-lookup"><span data-stu-id="85530-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85530-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="85530-125">Remarks</span></span>

<span data-ttu-id="85530-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="85530-126">This element is optional.</span></span>
  
<span data-ttu-id="85530-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="85530-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="85530-128">Пример</span><span class="sxs-lookup"><span data-stu-id="85530-128">Example</span></span>

<span data-ttu-id="85530-129">В приведенном ниже примере запроса показано, как задать элемент **инклудемимеконтент** .</span><span class="sxs-lookup"><span data-stu-id="85530-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="85530-130">Атрибут идентификатора вложения усекается для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="85530-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85530-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="85530-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85530-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="85530-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85530-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="85530-133">Schema Name</span></span>  <br/> |<span data-ttu-id="85530-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="85530-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="85530-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="85530-135">Validation File</span></span>  <br/> |<span data-ttu-id="85530-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="85530-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85530-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="85530-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="85530-138">False</span><span class="sxs-lookup"><span data-stu-id="85530-138">False</span></span>  <br/> |
   

