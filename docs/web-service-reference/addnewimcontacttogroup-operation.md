---
title: Операция AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Найдите сведения о веб-служб Exchange AddNewImContactToGroup операции.
ms.openlocfilehash: f75b89dbb6e948431d56acb9baa93fe4d4a1d939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761351"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="efdd6-103">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="efdd6-104">Найдите сведения о **AddNewImContactToGroup** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="efdd6-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="efdd6-105">Операция **AddNewImContactToGroup** добавляет новый контакт для обмена мгновенными сообщениями (IM) группы.</span><span class="sxs-lookup"><span data-stu-id="efdd6-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="efdd6-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="efdd6-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="efdd6-107">С помощью операции AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="efdd6-108">Операция **AddNewImContactToGroup** принимает следующие три аргумента для добавления нового контакта в группу обмена мгновенными Сообщениями:</span><span class="sxs-lookup"><span data-stu-id="efdd6-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="efdd6-109">Свойство **ImAddress** - определяет адрес обмена мгновенными Сообщениями контакта.</span><span class="sxs-lookup"><span data-stu-id="efdd6-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="efdd6-110">Это свойство является обязательным.</span><span class="sxs-lookup"><span data-stu-id="efdd6-110">This property is required.</span></span> 
    
- <span data-ttu-id="efdd6-111">Свойство **DisplayName** — определяет отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="efdd6-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="efdd6-112">Свойство **GroupId** - идентифицирует группу, что контакт.</span><span class="sxs-lookup"><span data-stu-id="efdd6-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="efdd6-113">Эта операция возвращает пользователя контактного лица, который был добавлен в группу.</span><span class="sxs-lookup"><span data-stu-id="efdd6-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="efdd6-114">Заголовки SOAP AddNewImContactToGroup операции</span><span class="sxs-lookup"><span data-stu-id="efdd6-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="efdd6-115">Операция **AddNewImContactToGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="efdd6-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="efdd6-116">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="efdd6-116">**Header name**</span></span>|<span data-ttu-id="efdd6-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="efdd6-117">**Element**</span></span>|<span data-ttu-id="efdd6-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="efdd6-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="efdd6-119">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="efdd6-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="efdd6-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="efdd6-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="efdd6-121">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="efdd6-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="efdd6-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="efdd6-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="efdd6-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="efdd6-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="efdd6-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="efdd6-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="efdd6-125">Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="efdd6-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="efdd6-126">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="efdd6-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="efdd6-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="efdd6-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="efdd6-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="efdd6-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="efdd6-129">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="efdd6-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="efdd6-130">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="efdd6-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="efdd6-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="efdd6-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="efdd6-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="efdd6-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="efdd6-133">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="efdd6-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="efdd6-134">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="efdd6-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="efdd6-135">Пример запроса AddNewImContactToGroup операции: Добавление нового контакта обмена мгновенными Сообщениями в группу</span><span class="sxs-lookup"><span data-stu-id="efdd6-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="efdd6-136">Приведенный ниже запрос операции **AddNewImContactToGroup** показано, как добавить новый контакт в существующую группу обмена мгновенными Сообщениями.</span><span class="sxs-lookup"><span data-stu-id="efdd6-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="efdd6-137">В этом примере значение свойства **GroupId** был возвращен из результаты [операции AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="efdd6-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="efdd6-138">Свойство **ExchangeStoreId** содержит значение свойства **GroupId** .</span><span class="sxs-lookup"><span data-stu-id="efdd6-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="efdd6-139">Значение **GroupId** был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="efdd6-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="efdd6-140">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="efdd6-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="efdd6-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="efdd6-142">ImAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="efdd6-143">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="efdd6-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="efdd6-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="efdd6-145">Успешные операции ответа AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="efdd6-146">В следующем примере показано успешного ответа на запрос операции **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="efdd6-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="efdd6-147">Ответ содержит пользователя только что созданный контакт.</span><span class="sxs-lookup"><span data-stu-id="efdd6-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="efdd6-148">Контакт добавляется в папку экспресс-контакты в Exchange.</span><span class="sxs-lookup"><span data-stu-id="efdd6-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="efdd6-149">Идентификаторы URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="efdd6-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="efdd6-150">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="efdd6-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="efdd6-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="efdd6-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="efdd6-152">Пользователь</span><span class="sxs-lookup"><span data-stu-id="efdd6-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="efdd6-153">PersonaId</span><span class="sxs-lookup"><span data-stu-id="efdd6-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="efdd6-154">PersonaType</span><span class="sxs-lookup"><span data-stu-id="efdd6-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="efdd6-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="efdd6-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="efdd6-156">Отображаемое имя (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="efdd6-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="efdd6-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="efdd6-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="efdd6-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="efdd6-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="efdd6-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="efdd6-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="efdd6-161">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="efdd6-162">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="efdd6-163">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="efdd6-164">ImAddress (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="efdd6-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="efdd6-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="efdd6-166">Атрибуты (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="efdd6-167">Атрибуты (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="efdd6-168">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="efdd6-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="efdd6-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="efdd6-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="efdd6-170">IsWritable</span><span class="sxs-lookup"><span data-stu-id="efdd6-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="efdd6-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="efdd6-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="efdd6-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="efdd6-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="efdd6-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="efdd6-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="efdd6-174">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="efdd6-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="efdd6-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="efdd6-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="efdd6-176">Значение (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="efdd6-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="efdd6-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="efdd6-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="efdd6-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="efdd6-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="efdd6-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="efdd6-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="efdd6-180">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="efdd6-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="efdd6-181">Ошибка операции AddNewImContactToGroup ответа</span><span class="sxs-lookup"><span data-stu-id="efdd6-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="efdd6-182">В следующем примере показано ошибочный ответ на запрос операции **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="efdd6-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="efdd6-183">Это ответ на запрос на добавление контакта в группу, которая не находится в почтовый ящик инициатора.</span><span class="sxs-lookup"><span data-stu-id="efdd6-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="efdd6-184">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="efdd6-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="efdd6-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="efdd6-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="efdd6-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="efdd6-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="efdd6-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="efdd6-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="efdd6-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="efdd6-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="efdd6-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="efdd6-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="efdd6-190">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="efdd6-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="efdd6-191">См. также</span><span class="sxs-lookup"><span data-stu-id="efdd6-191">See also</span></span>



[<span data-ttu-id="efdd6-192">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="efdd6-193">Операция AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="efdd6-194">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="efdd6-195">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="efdd6-196">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="efdd6-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="efdd6-197">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="efdd6-197">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

