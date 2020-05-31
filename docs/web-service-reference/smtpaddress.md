---
title: SmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SmtpAddress
api_type:
- schema
ms.assetid: 779305a6-ad1e-424e-8a69-4e3bef61d787
description: Элемент SmtpAddress представляет SMTP-адрес учетной записи, используемой для олицетворения, или адрес получателя SMTP для запроса на общий доступ к календарю или контакту.
ms.openlocfilehash: 39588f0892cdcec819a1972547155730be5785f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835511"
---
# <a name="smtpaddress"></a><span data-ttu-id="ae674-103">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="ae674-103">SmtpAddress</span></span>

<span data-ttu-id="ae674-104">Элемент **SmtpAddress** представляет SMTP-адрес учетной записи, используемой для олицетворения, или адрес получателя SMTP для запроса на общий доступ к календарю или контакту.</span><span class="sxs-lookup"><span data-stu-id="ae674-104">The **SmtpAddress** element represents the Simple Mail Transfer Protocol (SMTP) address of an account to be used for impersonation or a Simple Mail Transfer Protocol (SMTP) recipient address of a calendar or contact sharing request.</span></span> 
  
```xml
<SmtpAddress/>
```

<span data-ttu-id="ae674-105">**смтпаддресстипе**</span><span class="sxs-lookup"><span data-stu-id="ae674-105">**SmtpAddressType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ae674-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ae674-106">Attributes and elements</span></span>

<span data-ttu-id="ae674-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ae674-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ae674-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ae674-108">Attributes</span></span>

<span data-ttu-id="ae674-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ae674-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ae674-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ae674-110">Child elements</span></span>

<span data-ttu-id="ae674-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="ae674-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ae674-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ae674-112">Parent elements</span></span>

|<span data-ttu-id="ae674-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ae674-113">**Element**</span></span>|<span data-ttu-id="ae674-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ae674-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ae674-115">коннектингсид</span><span class="sxs-lookup"><span data-stu-id="ae674-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="ae674-116">Представляет учетную запись для олицетворения при использовании заголовка SOAP Ексчанжеимперсонатион.</span><span class="sxs-lookup"><span data-stu-id="ae674-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="ae674-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ae674-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="ae674-118">инвалидреЦипиент</span><span class="sxs-lookup"><span data-stu-id="ae674-118">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="ae674-119">Представляет недопустимый получатель сообщения общего доступа к календарю или обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="ae674-119">Represents an invalid recipient for a calendar sharing or contact sharing message.</span></span>  <br/> |
|[<span data-ttu-id="ae674-120">Получатели (Аррайофсмтпаддресстипе)</span><span class="sxs-lookup"><span data-stu-id="ae674-120">Recipients (ArrayOfSmtpAddressType)</span></span>](recipients-arrayofsmtpaddresstype.md) <br/> |<span data-ttu-id="ae674-121">Представляет коллекцию получателей, которым будет предоставлен доступ к общей папке.</span><span class="sxs-lookup"><span data-stu-id="ae674-121">Represents a collection of recipients that will be granted access to the shared folder.</span></span>  <br/> |
|[<span data-ttu-id="ae674-122">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="ae674-122">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="ae674-123">Определяет запрос на получение идентификатора локальной папки указанной общей папки.</span><span class="sxs-lookup"><span data-stu-id="ae674-123">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ae674-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ae674-124">Text value</span></span>

<span data-ttu-id="ae674-125">Необходимо указать текстовое значение, представляющее SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="ae674-125">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ae674-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="ae674-126">Remarks</span></span>

<span data-ttu-id="ae674-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ae674-127">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ae674-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ae674-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ae674-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ae674-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ae674-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ae674-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ae674-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ae674-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="ae674-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ae674-132">Validation File</span></span>  <br/> |<span data-ttu-id="ae674-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ae674-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ae674-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ae674-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ae674-135">False</span><span class="sxs-lookup"><span data-stu-id="ae674-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ae674-136">См. также</span><span class="sxs-lookup"><span data-stu-id="ae674-136">See also</span></span>

- [<span data-ttu-id="ae674-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ae674-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

