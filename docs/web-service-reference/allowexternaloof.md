---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: Элемент AllowExternalOof содержит значение, указывающее которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе).
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761374"
---
# <a name="allowexternaloof"></a><span data-ttu-id="dd922-103">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="dd922-103">AllowExternalOof</span></span>

<span data-ttu-id="dd922-104">Элемент **AllowExternalOof** содержит значение, указывающее которому отправляются внешних сообщений об отсутствии на работе Office (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="dd922-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="dd922-105">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="dd922-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="dd922-106">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="dd922-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="dd922-107">**ExternalAudience**</span><span class="sxs-lookup"><span data-stu-id="dd922-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd922-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd922-108">Attributes and elements</span></span>

<span data-ttu-id="dd922-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd922-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd922-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd922-110">Attributes</span></span>

<span data-ttu-id="dd922-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd922-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd922-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd922-112">Child elements</span></span>

<span data-ttu-id="dd922-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd922-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd922-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd922-114">Parent elements</span></span>

|<span data-ttu-id="dd922-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd922-115">**Element**</span></span>|<span data-ttu-id="dd922-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd922-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd922-117">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="dd922-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="dd922-118">Содержит параметры об отсутствии на работе для пользователя и результатов ответа.</span><span class="sxs-lookup"><span data-stu-id="dd922-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd922-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd922-119">Text value</span></span>

<span data-ttu-id="dd922-p101">Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="dd922-p101">A text value is required for this element. The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="dd922-122">**Значение**</span><span class="sxs-lookup"><span data-stu-id="dd922-122">**Value**</span></span>|<span data-ttu-id="dd922-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd922-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd922-124">**None**</span><span class="sxs-lookup"><span data-stu-id="dd922-124">**None**</span></span> <br/> |<span data-ttu-id="dd922-125">Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения пользователю, не получат внешнего ответа сообщение об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="dd922-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="dd922-126">**Известные**</span><span class="sxs-lookup"><span data-stu-id="dd922-126">**Known**</span></span> <br/> |<span data-ttu-id="dd922-127">Отправители электронной почты за пределами организации пользователя почтового ящика, которые отправляют сообщения, чтобы пользователь получит только внешние ответа сообщение об отсутствии на работе Если отправитель входит в Exchange пользователя хранить список контактов.</span><span class="sxs-lookup"><span data-stu-id="dd922-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="dd922-128">**All**</span><span class="sxs-lookup"><span data-stu-id="dd922-128">**All**</span></span> <br/> |<span data-ttu-id="dd922-129">Отправители электронной почты за пределами организации пользователя почтового ящика, отправлять сообщения для пользователя будет получать внешние ответа сообщение об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="dd922-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd922-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd922-130">Remarks</span></span>

<span data-ttu-id="dd922-131">Этот элемент использует совместно с типом элемента [ExternalAudience](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="dd922-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="dd922-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dd922-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd922-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dd922-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd922-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dd922-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dd922-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dd922-135">Schema Name</span></span>  <br/> |<span data-ttu-id="dd922-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="dd922-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dd922-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dd922-137">Validation File</span></span>  <br/> |<span data-ttu-id="dd922-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="dd922-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dd922-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dd922-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="dd922-140">False</span><span class="sxs-lookup"><span data-stu-id="dd922-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd922-141">См. также</span><span class="sxs-lookup"><span data-stu-id="dd922-141">See also</span></span>

- [<span data-ttu-id="dd922-142">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="dd922-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="dd922-143">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="dd922-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

