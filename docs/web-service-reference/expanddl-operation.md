---
title: Операция ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: Операция ExpandDL предоставляет полного контроля членства списков рассылки.
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762437"
---
# <a name="expanddl-operation"></a><span data-ttu-id="b435e-103">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="b435e-103">ExpandDL operation</span></span>

<span data-ttu-id="b435e-104">Операция ExpandDL предоставляет полного контроля членства списков рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="b435e-105">С помощью ExpandDL веб-метода</span><span class="sxs-lookup"><span data-stu-id="b435e-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="b435e-106">Операция ExpandDL использует веб-службы, размещенной в Exchange.asmx.</span><span class="sxs-lookup"><span data-stu-id="b435e-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="b435e-107">Этот метод веб-службы принимает элемент [почтового ящика](mailbox.md) , который может содержать дочерний элемент [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) расширения открытый список рассылки либо [ItemId](itemid.md) дочернего элемента для расширения частной список рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="b435e-108">Открытые списки рассылки могут быть развернуты с помощью одного из следующих:</span><span class="sxs-lookup"><span data-stu-id="b435e-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="b435e-109">Псевдоним списка рассылки</span><span class="sxs-lookup"><span data-stu-id="b435e-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="b435e-110">Адрес Simple Mail Transfer Protocol (SMTP)</span><span class="sxs-lookup"><span data-stu-id="b435e-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="b435e-111">X400</span><span class="sxs-lookup"><span data-stu-id="b435e-111">X400</span></span>
    
4. <span data-ttu-id="b435e-112">X500</span><span class="sxs-lookup"><span data-stu-id="b435e-112">X500</span></span>
    
5. <span data-ttu-id="b435e-113">Адрес прежних версий Exchange</span><span class="sxs-lookup"><span data-stu-id="b435e-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="b435e-114">Имя списка рассылки</span><span class="sxs-lookup"><span data-stu-id="b435e-114">The distribution list name</span></span>
    
7. <span data-ttu-id="b435e-115">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="b435e-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="b435e-116">Отображаемые имена не являются уникальными.</span><span class="sxs-lookup"><span data-stu-id="b435e-116">Display names are not unique.</span></span> <span data-ttu-id="b435e-117">Несколько учетных записей могут совместно использовать же отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b435e-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b435e-118">Замечания</span><span class="sxs-lookup"><span data-stu-id="b435e-118">Remarks</span></span>

<span data-ttu-id="b435e-119">Расширения рекурсивный не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b435e-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="b435e-120">Можно развернуть только один список, в одном вызове.</span><span class="sxs-lookup"><span data-stu-id="b435e-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="b435e-121">Если более одного списка рассылки соответствующие критериям, веб-службы отчетов об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b435e-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="b435e-122">Клиентское приложение может использовать разрешения неоднозначных имен (ANR) для поиска неоднозначные рассылки список, а затем выбрать правильный адрес электронной почты из списка рассылки необходимые как параметр [ExpandDL операции](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b435e-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="b435e-123">Для получения дополнительных сведений см [ResolveNames операции](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b435e-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="b435e-124">Открытые списки рассылки, находятся в Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b435e-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="b435e-125">Они могут быть любая группа рассылки с включенной поддержкой почты или динамической.</span><span class="sxs-lookup"><span data-stu-id="b435e-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="b435e-126">Группы не должен быть скрыт из списка адресов и каждый элемент должен иметь адрес электронной почты не пуста.</span><span class="sxs-lookup"><span data-stu-id="b435e-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="b435e-127">Члены списка рассылки могут быть пользователи с включенной поддержкой почты и контакты, общих папок и списков рассылки с включенной поддержкой почты и динамические группы.</span><span class="sxs-lookup"><span data-stu-id="b435e-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="b435e-128">Частные списки рассылки, находятся в папке «Контакты» из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b435e-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="b435e-129">Частные списки рассылки не имеют адреса электронной почты, поэтому их идентификаторы элемента хранилища используются в запросе ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="b435e-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="b435e-130">Члены списка рассылки закрытый может быть любого пользователя с включенной поддержкой почты, контакты или списки рассылки из службы каталогов Active Directory или контактов или частные списки рассылки из папки Контакты.</span><span class="sxs-lookup"><span data-stu-id="b435e-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="b435e-131">Для контактов или частные списки рассылки идентификаторы элементов возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="b435e-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="b435e-132">Можно использовать для получения сведений об объекте или чтобы развернуть членство в списке рассылки закрытый.</span><span class="sxs-lookup"><span data-stu-id="b435e-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="b435e-133">Пример запроса ExpandDL Private списка рассылки</span><span class="sxs-lookup"><span data-stu-id="b435e-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="b435e-134">Описание</span><span class="sxs-lookup"><span data-stu-id="b435e-134">Description</span></span>

<span data-ttu-id="b435e-135">В следующем примере запрос ExpandDL показано, как для формирования запроса разверните список рассылки закрытый.</span><span class="sxs-lookup"><span data-stu-id="b435e-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="b435e-136">Программа</span><span class="sxs-lookup"><span data-stu-id="b435e-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b435e-137">Комментарии</span><span class="sxs-lookup"><span data-stu-id="b435e-137">Comments</span></span>

<span data-ttu-id="b435e-138">Разверните список рассылки закрытый элемент [почтового ящика](mailbox.md) будет содержать элемент [ItemId](itemid.md) , определяющий список рассылки закрытый в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="b435e-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="b435e-139">Пример запроса ExpandDL общедоступных списка рассылки</span><span class="sxs-lookup"><span data-stu-id="b435e-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="b435e-140">Описание</span><span class="sxs-lookup"><span data-stu-id="b435e-140">Description</span></span>

<span data-ttu-id="b435e-141">В следующем примере запрос ExpandDL показано, как для формирования запроса, чтобы развернуть открытый список рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="b435e-142">В примере показано использование отображаемое имя, чтобы развернуть список рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="b435e-143">Программа</span><span class="sxs-lookup"><span data-stu-id="b435e-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="b435e-144">Комментарии</span><span class="sxs-lookup"><span data-stu-id="b435e-144">Comments</span></span>

<span data-ttu-id="b435e-145">Ответ на этот запрос будет содержать элементы **почтового ящика** , чтобы указать каждого почтового ящика в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="b435e-146">Если список рассылки содержится в список рассылки, раскрытие списков рассылки отдельные необходимо выполнить на список внедренных рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="b435e-147">Если этот список рассылки не имеет членов или список рассылки запрошенные не существует, атрибут **ResponseClass** будет содержать значение, равное успеха.</span><span class="sxs-lookup"><span data-stu-id="b435e-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="b435e-148">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="b435e-148">Request elements</span></span>

<span data-ttu-id="b435e-149">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b435e-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="b435e-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="b435e-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="b435e-151">Mailbox</span><span class="sxs-lookup"><span data-stu-id="b435e-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="b435e-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) используется для идентификации открытые списки рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="b435e-153">Элемент [ItemId](itemid.md) используется для идентификации частные списки рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b435e-154">Схема, описывающая эти элементы находится в виртуальном каталоге EWS компьютера, на котором работает MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b435e-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="b435e-155">Пример успешного ответа ExpandDL</span><span class="sxs-lookup"><span data-stu-id="b435e-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="b435e-156">Описание</span><span class="sxs-lookup"><span data-stu-id="b435e-156">Description</span></span>

<span data-ttu-id="b435e-157">В следующем примере ответа ExpandDL показано ответа на запрос, описанных выше.</span><span class="sxs-lookup"><span data-stu-id="b435e-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="b435e-158">Раскрытие списка рассылки описываются следующие:</span><span class="sxs-lookup"><span data-stu-id="b435e-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="b435e-159">Количество членов списка рассылки, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="b435e-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="b435e-160">Содержит ли ответ всех членов списка рассылки.</span><span class="sxs-lookup"><span data-stu-id="b435e-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="b435e-161">Имя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b435e-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="b435e-162">Адрес электронной почты для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b435e-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="b435e-163">Тип маршрутизации для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b435e-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="b435e-164">Тип почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b435e-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="b435e-165">Имя списка рассылки не включенных в ответ; Таким образом вы должны отслеживать связи имя запроса.</span><span class="sxs-lookup"><span data-stu-id="b435e-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b435e-166">Программа</span><span class="sxs-lookup"><span data-stu-id="b435e-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="b435e-167">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="b435e-167">Successful response elements</span></span>

<span data-ttu-id="b435e-168">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b435e-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="b435e-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b435e-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b435e-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="b435e-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="b435e-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b435e-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b435e-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b435e-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="b435e-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b435e-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b435e-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="b435e-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="b435e-175">Mailbox</span><span class="sxs-lookup"><span data-stu-id="b435e-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="b435e-176">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b435e-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="b435e-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="b435e-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="b435e-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="b435e-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="b435e-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="b435e-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="b435e-180">Чтобы найти другие параметры в сообщении ответа операция ExpandDL, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="b435e-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="b435e-181">Запустите в элементе [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="b435e-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="b435e-182">Ошибка ExpandDL ответа</span><span class="sxs-lookup"><span data-stu-id="b435e-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="b435e-183">Описание</span><span class="sxs-lookup"><span data-stu-id="b435e-183">Description</span></span>

<span data-ttu-id="b435e-184">В следующем примере показано ошибочный ответ на запрос ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="b435e-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b435e-185">Программа</span><span class="sxs-lookup"><span data-stu-id="b435e-185">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="b435e-186">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="b435e-186">Error response elements</span></span>

<span data-ttu-id="b435e-187">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="b435e-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="b435e-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="b435e-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="b435e-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="b435e-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="b435e-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b435e-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="b435e-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b435e-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="b435e-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="b435e-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="b435e-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b435e-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="b435e-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b435e-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="b435e-195">Чтобы найти другие параметры в сообщении ответа операция ExpandDL, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="b435e-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="b435e-196">Запустите в элементе [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="b435e-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="b435e-197">См. также</span><span class="sxs-lookup"><span data-stu-id="b435e-197">See also</span></span>

- [<span data-ttu-id="b435e-198">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="b435e-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="b435e-199">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b435e-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

