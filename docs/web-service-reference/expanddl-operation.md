---
title: Операция ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: Операция ExpandDL предоставляет полное членство в списках рассылки.
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454052"
---
# <a name="expanddl-operation"></a><span data-ttu-id="a5fdf-103">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-103">ExpandDL operation</span></span>

<span data-ttu-id="a5fdf-104">Операция ExpandDL предоставляет полное членство в списках рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="a5fdf-105">Использование веб-метода ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="a5fdf-106">Операция ExpandDL использует веб-службу, размещенную в Exchange. asmx.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="a5fdf-107">Этот метод веб-службы принимает элемент [почтового ящика](mailbox.md) , который может содержать дочерний элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) для расширения общедоступного списка рассылки или дочернего элемента [ItemId](itemid.md) для расширения частного списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="a5fdf-108">Общедоступные списки рассылки можно развернуть с помощью одного из следующих компонентов:</span><span class="sxs-lookup"><span data-stu-id="a5fdf-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="a5fdf-109">Псевдоним списка рассылки</span><span class="sxs-lookup"><span data-stu-id="a5fdf-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="a5fdf-110">SMTP-адрес</span><span class="sxs-lookup"><span data-stu-id="a5fdf-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="a5fdf-111">X400</span><span class="sxs-lookup"><span data-stu-id="a5fdf-111">X400</span></span>
    
4. <span data-ttu-id="a5fdf-112">Х</span><span class="sxs-lookup"><span data-stu-id="a5fdf-112">X500</span></span>
    
5. <span data-ttu-id="a5fdf-113">Устаревший адрес Exchange</span><span class="sxs-lookup"><span data-stu-id="a5fdf-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="a5fdf-114">Имя списка рассылки</span><span class="sxs-lookup"><span data-stu-id="a5fdf-114">The distribution list name</span></span>
    
7. <span data-ttu-id="a5fdf-115">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="a5fdf-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="a5fdf-116">Отображаемые имена не являются уникальными.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-116">Display names are not unique.</span></span> <span data-ttu-id="a5fdf-117">Несколько учетных записей могут иметь одно и то же отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a5fdf-118">Примечания</span><span class="sxs-lookup"><span data-stu-id="a5fdf-118">Remarks</span></span>

<span data-ttu-id="a5fdf-119">Рекурсивное расширение не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="a5fdf-120">В одном вызове можно развернуть только один список рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="a5fdf-121">Если критерию отвечает несколько списков рассылки, веб-служба сообщает об ошибке.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="a5fdf-122">Клиентское приложение может использовать разрешение неоднозначных имен, чтобы найти неоднозначные списки рассылки, а затем выбрать правильный адрес электронной почты требуемого списка рассылки в качестве параметра для [операции ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a5fdf-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="a5fdf-123">Дополнительные сведения см. в разделе [Operation ResolveNames Operation](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a5fdf-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="a5fdf-124">Общедоступные списки рассылки находятся в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="a5fdf-125">Можно использовать любую группу рассылки с поддержкой почты или динамическую группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="a5fdf-126">Группу не следует скрывать из списка адресов, а у каждого участника должен быть непустой адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="a5fdf-127">Членами этого списка рассылки могут быть пользователи и контакты, общедоступные папки и списки рассылки с поддержкой почты и динамические группы.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="a5fdf-128">Частные списки рассылки находятся в папке "Контакты" в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="a5fdf-129">Частные списки рассылки не имеют адресов электронной почты, поэтому их идентификаторы элементов хранилища используются в запросе ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="a5fdf-130">Членами частного списка рассылки может быть любой пользователь с включенной поддержкой почты, контакты или списки рассылки из Active Directory, а также списки контактов или частных рассылки из папки "Контакты" пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="a5fdf-131">Для контактов или частных списков рассылки в ответе возвращаются идентификаторы элементов.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="a5fdf-132">Этот параметр можно использовать для получения сведений о объекте или для расширения членства в частном списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="a5fdf-133">Пример запроса частного списка рассылки ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="a5fdf-134">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fdf-134">Description</span></span>

<span data-ttu-id="a5fdf-135">В приведенном ниже примере запроса ExpandDL показано, как сформировать запрос на развертывание частного списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="a5fdf-136">Код</span><span class="sxs-lookup"><span data-stu-id="a5fdf-136">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5fdf-137">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5fdf-137">Comments</span></span>

<span data-ttu-id="a5fdf-138">Чтобы развернуть частный список рассылки, элемент [Mailbox](mailbox.md) будет содержать элемент [ItemId](itemid.md) , определяющий частный список рассылки в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="a5fdf-139">Пример общего списка рассылки ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="a5fdf-140">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fdf-140">Description</span></span>

<span data-ttu-id="a5fdf-141">В приведенном ниже примере запроса ExpandDL показано, как создать запрос для развертывания общедоступного списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="a5fdf-142">В этом примере показано использование отображаемого имени для развертывания списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="a5fdf-143">Код</span><span class="sxs-lookup"><span data-stu-id="a5fdf-143">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5fdf-144">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5fdf-144">Comments</span></span>

<span data-ttu-id="a5fdf-145">Ответ на этот запрос будет содержать элементы **почтовых ящиков** , которые определяют каждый почтовый ящик в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="a5fdf-146">Если список рассылки находится в списке рассылки, для внедренного списка рассылки должно выполняться отдельное расширение списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="a5fdf-147">Если в списке рассылки нет участников или запрошенный список рассылки не существует, атрибут **респонсекласс** будет содержать значение Success.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a5fdf-148">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="a5fdf-148">Request elements</span></span>

<span data-ttu-id="a5fdf-149">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5fdf-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a5fdf-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="a5fdf-151">Mailbox</span><span class="sxs-lookup"><span data-stu-id="a5fdf-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="a5fdf-152">[EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) используется для идентификации общедоступных списков рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="a5fdf-153">Элемент [ItemId](itemid.md) используется для идентификации частных списков рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="a5fdf-154">Схема, описывающая эти элементы, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Майкрософт Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="a5fdf-155">Пример успешного ответа ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="a5fdf-156">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fdf-156">Description</span></span>

<span data-ttu-id="a5fdf-157">В приведенном ниже примере ответа ExpandDL показан ответ на запрос, описанный выше.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="a5fdf-158">Раскрытие списка рассылки содержит следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="a5fdf-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="a5fdf-159">Количество членов списка рассылки, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="a5fdf-160">Содержит ли ответ все члены списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="a5fdf-161">Имя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="a5fdf-162">Адрес электронной почты почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="a5fdf-163">Тип маршрутизации для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="a5fdf-164">Тип почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a5fdf-165">Имя списка рассылки не включается в ответ; Поэтому необходимо следить за именем в запросе.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a5fdf-166">Код</span><span class="sxs-lookup"><span data-stu-id="a5fdf-166">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="a5fdf-167">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a5fdf-167">Successful response elements</span></span>

<span data-ttu-id="a5fdf-168">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5fdf-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a5fdf-169">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a5fdf-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a5fdf-170">експанддлреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5fdf-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="a5fdf-171">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a5fdf-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a5fdf-172">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a5fdf-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="a5fdf-173">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5fdf-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a5fdf-174">длекспансион</span><span class="sxs-lookup"><span data-stu-id="a5fdf-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="a5fdf-175">Mailbox</span><span class="sxs-lookup"><span data-stu-id="a5fdf-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="a5fdf-176">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a5fdf-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="a5fdf-177">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="a5fdf-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="a5fdf-178">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="a5fdf-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="a5fdf-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a5fdf-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="a5fdf-180">Чтобы найти другие параметры для ответного сообщения операции ExpandDL, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a5fdf-181">Начните с элемента [експанддлреспонсе](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a5fdf-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="a5fdf-182">Ответ об ошибке ExpandDL</span><span class="sxs-lookup"><span data-stu-id="a5fdf-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="a5fdf-183">Описание</span><span class="sxs-lookup"><span data-stu-id="a5fdf-183">Description</span></span>

<span data-ttu-id="a5fdf-184">В следующем примере показан ответ об ошибке для запроса ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="a5fdf-185">Код</span><span class="sxs-lookup"><span data-stu-id="a5fdf-185">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="a5fdf-186">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="a5fdf-186">Error response elements</span></span>

<span data-ttu-id="a5fdf-187">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5fdf-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a5fdf-188">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a5fdf-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a5fdf-189">експанддлреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5fdf-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="a5fdf-190">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a5fdf-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a5fdf-191">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a5fdf-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="a5fdf-192">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="a5fdf-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a5fdf-193">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5fdf-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a5fdf-194">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="a5fdf-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="a5fdf-195">Чтобы найти другие параметры для ответного сообщения операции ExpandDL, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="a5fdf-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a5fdf-196">Начните с элемента [експанддлреспонсе](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a5fdf-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a5fdf-197">См. также</span><span class="sxs-lookup"><span data-stu-id="a5fdf-197">See also</span></span>

- [<span data-ttu-id="a5fdf-198">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="a5fdf-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="a5fdf-199">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5fdf-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

