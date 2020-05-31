---
title: екстерналаудиенце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: Элемент Екстерналаудиенце задает или содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе).
ms.openlocfilehash: 836b0f6a5140a37e1584f571cb8e26534fe7a25f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762484"
---
# <a name="externalaudience"></a><span data-ttu-id="e985e-103">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="e985e-103">ExternalAudience</span></span>

<span data-ttu-id="e985e-104">Элемент **екстерналаудиенце** задает или содержит значение, определяющее отправку внешних сообщений об отсутствии на работе (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="e985e-104">The **ExternalAudience** element sets or contains a value that determines to whom external Out of Office (OOF) messages are sent.</span></span> 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 <span data-ttu-id="e985e-105">**екстерналаудиенце**</span><span class="sxs-lookup"><span data-stu-id="e985e-105">**ExternalAudience**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e985e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e985e-106">Attributes and elements</span></span>

<span data-ttu-id="e985e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e985e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e985e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e985e-108">Attributes</span></span>

<span data-ttu-id="e985e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e985e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e985e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e985e-110">Child elements</span></span>

<span data-ttu-id="e985e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e985e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e985e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e985e-112">Parent elements</span></span>

|<span data-ttu-id="e985e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e985e-113">**Element**</span></span>|<span data-ttu-id="e985e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e985e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e985e-115">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="e985e-115">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="e985e-116">Задает параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="e985e-116">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="e985e-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e985e-117">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="e985e-118">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="e985e-118">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="e985e-119">Содержит параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="e985e-119">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="e985e-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e985e-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e985e-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e985e-121">Text value</span></span>

<span data-ttu-id="e985e-p101">Для этого элемента требуется указать текстовое значение. В таблице ниже перечислены возможные варианты последнего.</span><span class="sxs-lookup"><span data-stu-id="e985e-p101">A text value is required for this element. The following table lists the possible values for this element.</span></span>
  
|<span data-ttu-id="e985e-124">**Значение**</span><span class="sxs-lookup"><span data-stu-id="e985e-124">**Value**</span></span>|<span data-ttu-id="e985e-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e985e-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e985e-126">**Нет**</span><span class="sxs-lookup"><span data-stu-id="e985e-126">**None**</span></span> <br/> |<span data-ttu-id="e985e-127">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, не будут получать ответ об отсутствии внешних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="e985e-127">E-mail senders outside the mailbox user's organization who send messages to the user will not receive an external OOF message response.</span></span>  <br/> |
|<span data-ttu-id="e985e-128">**Стандартных**</span><span class="sxs-lookup"><span data-stu-id="e985e-128">**Known**</span></span> <br/> |<span data-ttu-id="e985e-129">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, будут получать ответ о внешнем ответе на отсутствие ответа, если отправитель находится в списке контактов хранилища Exchange пользователя.</span><span class="sxs-lookup"><span data-stu-id="e985e-129">E-mail senders outside the mailbox user's organization who send messages to the user will only receive an external OOF message response if the sender is in the user's Exchange store contact list.</span></span>  <br/> |
|<span data-ttu-id="e985e-130">**All**</span><span class="sxs-lookup"><span data-stu-id="e985e-130">**All**</span></span> <br/> |<span data-ttu-id="e985e-131">Отправители электронной почты за пределами организации пользователя почтового ящика, который отправляет сообщения пользователю, получат сообщение о внешнем ответе на отсутствие.</span><span class="sxs-lookup"><span data-stu-id="e985e-131">E-mail senders outside the mailbox user's organization who send messages to the user will receive an external OOF message response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e985e-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="e985e-132">Remarks</span></span>

<span data-ttu-id="e985e-133">Этот элемент использует тот же тип, что и элемент [алловекстерналуф](allowexternaloof.md) .</span><span class="sxs-lookup"><span data-stu-id="e985e-133">This element shares the same type as the [AllowExternalOof](allowexternaloof.md) element.</span></span> 
  
<span data-ttu-id="e985e-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e985e-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e985e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="e985e-135">Example</span></span>

<span data-ttu-id="e985e-136">В приведенном ниже примере запроса SetUserOofSettings задается для параметра Уфстате значение **Enabled**, устанавливается для внешней аудитории значение " **все**", устанавливается время бездействия в 10 дней и задаются внутренние и внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="e985e-136">The following example of a SetUserOofSettings request sets the OoFState to **Enabled**, sets the external audience to **All**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="e985e-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e985e-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e985e-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e985e-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e985e-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e985e-139">Schema Name</span></span>  <br/> |<span data-ttu-id="e985e-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e985e-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="e985e-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e985e-141">Validation File</span></span>  <br/> |<span data-ttu-id="e985e-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e985e-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e985e-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e985e-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="e985e-144">False</span><span class="sxs-lookup"><span data-stu-id="e985e-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e985e-145">См. также</span><span class="sxs-lookup"><span data-stu-id="e985e-145">See also</span></span>



[<span data-ttu-id="e985e-146">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e985e-146">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="e985e-147">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="e985e-147">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

