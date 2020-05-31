---
title: Операция AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Поиск сведений о AddNewImContactToGroupной операции EWS.
ms.openlocfilehash: f75b89dbb6e948431d56acb9baa93fe4d4a1d939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761351"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="e0eea-103">Операция AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="e0eea-104">Поиск сведений о **AddNewImContactToGroupной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="e0eea-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="e0eea-105">Операция **AddNewImContactToGroup** добавляет новый контакт в группу мгновенных сообщений (IM).</span><span class="sxs-lookup"><span data-stu-id="e0eea-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="e0eea-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e0eea-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="e0eea-107">Использование операции AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="e0eea-108">Для добавления нового контакта в группу обмена мгновенными сообщениями в операции **AddNewImContactToGroup** используются три указанных ниже аргумента.</span><span class="sxs-lookup"><span data-stu-id="e0eea-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="e0eea-109">Свойство " **Address** " — определяет адрес для обмена мгновенными сообщениями контакта.</span><span class="sxs-lookup"><span data-stu-id="e0eea-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="e0eea-110">Это свойство является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e0eea-110">This property is required.</span></span> 
    
- <span data-ttu-id="e0eea-111">Свойство **DisplayName** — определяет отображаемое имя контакта.</span><span class="sxs-lookup"><span data-stu-id="e0eea-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="e0eea-112">**GroupId** свойство — определяет группу, в которую добавляется контакт.</span><span class="sxs-lookup"><span data-stu-id="e0eea-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="e0eea-113">Эта операция возвращает пользователя контакта, который был добавлен в группу.</span><span class="sxs-lookup"><span data-stu-id="e0eea-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="e0eea-114">Заголовки SOAP операции AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="e0eea-115">Операция **AddNewImContactToGroup** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="e0eea-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e0eea-116">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="e0eea-116">**Header name**</span></span>|<span data-ttu-id="e0eea-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e0eea-117">**Element**</span></span>|<span data-ttu-id="e0eea-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e0eea-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e0eea-119">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="e0eea-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="e0eea-120">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="e0eea-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e0eea-121">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="e0eea-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="e0eea-122">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="e0eea-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0eea-123">**маилбокскултуре**</span><span class="sxs-lookup"><span data-stu-id="e0eea-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="e0eea-124">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="e0eea-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e0eea-125">Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="e0eea-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="e0eea-126">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="e0eea-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0eea-127">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="e0eea-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e0eea-128">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="e0eea-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e0eea-129">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="e0eea-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e0eea-130">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="e0eea-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0eea-131">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="e0eea-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e0eea-132">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="e0eea-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e0eea-133">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="e0eea-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e0eea-134">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="e0eea-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="e0eea-135">Пример запроса операции AddNewImContactToGroup: Добавление нового контакта для обмена мгновенными сообщениями в группу</span><span class="sxs-lookup"><span data-stu-id="e0eea-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="e0eea-136">В следующем примере запроса операции **AddNewImContactToGroup** показано, как добавить новый контакт в существующую группу обмена мгновенными сообщениями.</span><span class="sxs-lookup"><span data-stu-id="e0eea-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="e0eea-137">Значение свойства **groupId** для этого примера было возвращено из результатов [операции AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="e0eea-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="e0eea-138">Свойство **ексчанжестореид** содержит значение свойства **groupId** .</span><span class="sxs-lookup"><span data-stu-id="e0eea-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
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
> <span data-ttu-id="e0eea-139">Значение **groupId** было сокращено, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="e0eea-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="e0eea-140">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0eea-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0eea-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="e0eea-142">Адрес (String)</span><span class="sxs-lookup"><span data-stu-id="e0eea-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="e0eea-143">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="e0eea-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="e0eea-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="e0eea-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="e0eea-145">Успешный отклик операции AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="e0eea-146">В следующем примере показан успешный ответ на запрос операции **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="e0eea-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="e0eea-147">Ответ содержит пользователя созданного контакта.</span><span class="sxs-lookup"><span data-stu-id="e0eea-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="e0eea-148">Контакт будет добавлен в папку "Быстрые контакты" в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0eea-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e0eea-149">Идентификаторы сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e0eea-149">Identifiers have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="e0eea-150">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0eea-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0eea-151">аддневимконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="e0eea-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="e0eea-152">Роль</span><span class="sxs-lookup"><span data-stu-id="e0eea-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="e0eea-153">персонаид</span><span class="sxs-lookup"><span data-stu-id="e0eea-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="e0eea-154">персонатипе</span><span class="sxs-lookup"><span data-stu-id="e0eea-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="e0eea-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="e0eea-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="e0eea-156">DisplayName (строка)</span><span class="sxs-lookup"><span data-stu-id="e0eea-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="e0eea-157">дисплайнамефирстласт</span><span class="sxs-lookup"><span data-stu-id="e0eea-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="e0eea-158">дисплайнамеластфирст</span><span class="sxs-lookup"><span data-stu-id="e0eea-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="e0eea-159">филеасид</span><span class="sxs-lookup"><span data-stu-id="e0eea-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="e0eea-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e0eea-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="e0eea-161">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e0eea-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="e0eea-162">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="e0eea-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="e0eea-163">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e0eea-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="e0eea-164">Адрес (String)</span><span class="sxs-lookup"><span data-stu-id="e0eea-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="e0eea-165">релеванцескоре</span><span class="sxs-lookup"><span data-stu-id="e0eea-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="e0eea-166">Атрибуты (Аррайофперсонааттрибутионстипе)</span><span class="sxs-lookup"><span data-stu-id="e0eea-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="e0eea-167">Атрибуты (Персонааттрибутионтипе)</span><span class="sxs-lookup"><span data-stu-id="e0eea-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="e0eea-168">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="e0eea-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="e0eea-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="e0eea-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="e0eea-170">Доступный для записи</span><span class="sxs-lookup"><span data-stu-id="e0eea-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="e0eea-171">искуиккконтакт</span><span class="sxs-lookup"><span data-stu-id="e0eea-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="e0eea-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="e0eea-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="e0eea-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="e0eea-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="e0eea-174">DisplayName</span><span class="sxs-lookup"><span data-stu-id="e0eea-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="e0eea-175">стрингаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="e0eea-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="e0eea-176">Значение (Аррайофстрингвалуетипе)</span><span class="sxs-lookup"><span data-stu-id="e0eea-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="e0eea-177">филеасидс</span><span class="sxs-lookup"><span data-stu-id="e0eea-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="e0eea-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="e0eea-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="e0eea-179">емаиладдрессаттрибутедвалуе</span><span class="sxs-lookup"><span data-stu-id="e0eea-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="e0eea-180">Адреса</span><span class="sxs-lookup"><span data-stu-id="e0eea-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="e0eea-181">Ответ об ошибке операции AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="e0eea-182">В следующем примере показан ответ об ошибке для запроса операции **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="e0eea-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="e0eea-183">Это ответ на запрос на добавление контакта в группу, которая не находится в почтовом ящике запросившего.</span><span class="sxs-lookup"><span data-stu-id="e0eea-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
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

<span data-ttu-id="e0eea-184">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e0eea-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0eea-185">аддневимконтакттограупреспонсе</span><span class="sxs-lookup"><span data-stu-id="e0eea-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="e0eea-186">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="e0eea-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e0eea-187">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="e0eea-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e0eea-188">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="e0eea-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="e0eea-189">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="e0eea-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="e0eea-190">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="e0eea-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e0eea-191">См. также</span><span class="sxs-lookup"><span data-stu-id="e0eea-191">See also</span></span>



[<span data-ttu-id="e0eea-192">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="e0eea-193">Операция AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="e0eea-194">Операция AddImGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="e0eea-195">Операция RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="e0eea-196">Операция SetImGroup</span><span class="sxs-lookup"><span data-stu-id="e0eea-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="e0eea-197">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="e0eea-197">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

