---
title: алловекстерналуф
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
description: Элемент Алловекстерналуф содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе).
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464814"
---
# <a name="allowexternaloof"></a><span data-ttu-id="d7b07-103">алловекстерналуф</span><span class="sxs-lookup"><span data-stu-id="d7b07-103">AllowExternalOof</span></span>

<span data-ttu-id="d7b07-104">Элемент **алловекстерналуф** содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="d7b07-104">The **AllowExternalOof** element contains a value that identifies to whom external Out of Office (OOF) messages are sent.</span></span> 
  
- [<span data-ttu-id="d7b07-105">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d7b07-105">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
  
- [<span data-ttu-id="d7b07-106">алловекстерналуф</span><span class="sxs-lookup"><span data-stu-id="d7b07-106">AllowExternalOof</span></span>](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 <span data-ttu-id="d7b07-107">**екстерналаудиенце**</span><span class="sxs-lookup"><span data-stu-id="d7b07-107">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d7b07-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d7b07-108">Attributes and elements</span></span>

<span data-ttu-id="d7b07-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d7b07-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d7b07-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d7b07-110">Attributes</span></span>

<span data-ttu-id="d7b07-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d7b07-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d7b07-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d7b07-112">Child elements</span></span>

<span data-ttu-id="d7b07-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d7b07-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d7b07-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d7b07-114">Parent elements</span></span>

|<span data-ttu-id="d7b07-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d7b07-115">**Element**</span></span>|<span data-ttu-id="d7b07-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7b07-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d7b07-117">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d7b07-117">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="d7b07-118">Содержит результаты ответа и параметры отсутствия на отсутствие для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7b07-118">Contains the response results and the OOF settings for a user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d7b07-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d7b07-119">Text value</span></span>

<span data-ttu-id="d7b07-p101">Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="d7b07-p101">A text value is required for this element. The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="d7b07-122">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d7b07-122">**Value**</span></span>|<span data-ttu-id="d7b07-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d7b07-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d7b07-124">**Нет**</span><span class="sxs-lookup"><span data-stu-id="d7b07-124">**None**</span></span> <br/> |<span data-ttu-id="d7b07-125">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, не будут получать ответ об отсутствии внешних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="d7b07-125">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="d7b07-126">**Стандартных**</span><span class="sxs-lookup"><span data-stu-id="d7b07-126">**Known**</span></span> <br/> |<span data-ttu-id="d7b07-127">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, будут получать ответ о внешнем ответе на отсутствие ответа, если отправитель находится в списке контактов хранилища Exchange пользователя.</span><span class="sxs-lookup"><span data-stu-id="d7b07-127">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="d7b07-128">**All**</span><span class="sxs-lookup"><span data-stu-id="d7b07-128">**All**</span></span> <br/> |<span data-ttu-id="d7b07-129">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, получат сообщение о внешнем ответе на отсутствие.</span><span class="sxs-lookup"><span data-stu-id="d7b07-129">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d7b07-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="d7b07-130">Remarks</span></span>

<span data-ttu-id="d7b07-131">Этот элемент использует тот же тип, что и элемент [екстерналаудиенце](externalaudience.md) .</span><span class="sxs-lookup"><span data-stu-id="d7b07-131">This element shares the same type as the [ExternalAudience](externalaudience.md) element.</span></span> 
  
<span data-ttu-id="d7b07-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d7b07-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d7b07-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d7b07-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d7b07-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d7b07-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d7b07-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d7b07-135">Schema Name</span></span>  <br/> |<span data-ttu-id="d7b07-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="d7b07-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d7b07-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d7b07-137">Validation File</span></span>  <br/> |<span data-ttu-id="d7b07-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d7b07-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d7b07-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d7b07-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="d7b07-140">False</span><span class="sxs-lookup"><span data-stu-id="d7b07-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d7b07-141">См. также</span><span class="sxs-lookup"><span data-stu-id="d7b07-141">See also</span></span>

- [<span data-ttu-id="d7b07-142">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d7b07-142">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md) 
- [<span data-ttu-id="d7b07-143">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d7b07-143">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

