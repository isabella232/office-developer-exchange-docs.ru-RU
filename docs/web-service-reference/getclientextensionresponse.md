---
title: жетклиентекстенсионреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4b1aba-a55d-4d64-ac80-5d4e6c4e72bd
description: Элемент Жетклиентекстенсионреспонсе содержит ответ для получения сведений о конфигурации приложения.
ms.openlocfilehash: 65c1995fe75b3894607d27ed65548fbbdce0664a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459520"
---
# <a name="getclientextensionresponse"></a><span data-ttu-id="6e420-103">жетклиентекстенсионреспонсе</span><span class="sxs-lookup"><span data-stu-id="6e420-103">GetClientExtensionResponse</span></span>

<span data-ttu-id="6e420-104">Элемент **жетклиентекстенсионреспонсе** содержит ответ для получения сведений о конфигурации приложения.</span><span class="sxs-lookup"><span data-stu-id="6e420-104">The **GetClientExtensionResponse** element contains the response to get configuration information about an app.</span></span> 
  
```XML
<GetClientExtensionResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ClientExtensions/>
   <RawMasterTableXml/>
</GetClientExtensionResponse>
```

 <span data-ttu-id="6e420-105">**клиентекстенсионреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="6e420-105">**ClientExtensionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e420-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e420-106">Attributes and elements</span></span>

<span data-ttu-id="6e420-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6e420-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e420-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e420-108">Attributes</span></span>

<span data-ttu-id="6e420-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6e420-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e420-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e420-110">Child elements</span></span>

<span data-ttu-id="6e420-111">[Мессажетекст](messagetext.md)  |  [Респонсекоде](responsecode.md)  |  [Дескриптивелинккэй](descriptivelinkkey.md)  |  [Мессажексмл](messagexml.md)  |  [Клиентекстенсионс](clientextensions.md)  |  [Равмастертаблексмл](rawmastertablexml.md)</span><span class="sxs-lookup"><span data-stu-id="6e420-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [ClientExtensions](clientextensions.md) | [RawMasterTableXml](rawmastertablexml.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e420-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e420-112">Parent elements</span></span>

<span data-ttu-id="6e420-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e420-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e420-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="6e420-114">Remarks</span></span>

<span data-ttu-id="6e420-115">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6e420-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6e420-116">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e420-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e420-117">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e420-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e420-118">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e420-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e420-119">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e420-119">Schema name</span></span>  <br/> |<span data-ttu-id="6e420-120">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6e420-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e420-121">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e420-121">Validation file</span></span>  <br/> |<span data-ttu-id="6e420-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6e420-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e420-123">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e420-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6e420-124">false</span><span class="sxs-lookup"><span data-stu-id="6e420-124">false</span></span>  <br/> |
   

