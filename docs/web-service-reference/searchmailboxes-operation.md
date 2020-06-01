---
title: Операция SearchMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a67c1d8-d021-4e68-aa62-35f7d9c2edc7
description: Поиск сведений о SearchMailboxesной операции EWS.
ms.openlocfilehash: 9ec7e9dd4ef17f22f236e64ca1fdbeb65e6e56fe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456776"
---
# <a name="searchmailboxes-operation"></a>Операция SearchMailboxes

> [!NOTE]
> Эта операция устарела и больше не поддерживается корпорацией Майкрософт.  В качестве замены используйте операцию [FindItem](finditem-operation.md) .

Поиск сведений о **SearchMailboxesной** операции EWS. 
  
Операция **SearchMailboxes** выполняет поиск в почтовых ящиках вхождений терминов в элементах почтового ящика. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-searchmailboxes-operation"></a>Использование операции SearchMailboxes

Для выполнения поиска в нескольких почтовых ящиках с помощью операции **SearchMailboxes** можно использовать несколько одновременных запросов поиска. Результаты могут представлять собой статистическую информацию о количестве выполняемых условий поиска или предварительном просмотре элементов, содержащих условия поиска. 
  
### <a name="searchmailboxes-operation-soap-headers"></a>Заголовки SOAP операции SearchMailboxes

Операция **SearchMailboxes** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Определяет роли сервера, необходимые для того, чтобы вызывающий абонент мог выполнить запрос. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="searchmailboxes-operation-request-example-search-mailboxes-for-number-of-search-term-hits"></a>Пример запроса операции SearchMailboxes: почтовые ящики поиска для количества совпадений со словами поиска

В приведенном ниже примере запроса операции **SearchMailboxes** показано, как использовать два разных запроса для поиска в трех разных почтовых ящиках статистические сведения о том, сколько раз термин отображается в каждом почтовом ящике. 
  
> [!NOTE]
> В этом примере элемент [Query](query.md) является пустым. В этом примере показано, как успешный запрос может содержать условия ошибки для каждой базы для поиска почтовых ящиков. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SearchMailboxes>
         <m:SearchQueries>
            <t:MailboxQuery>
               <t:Query>Test Item</t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=12311a742f0e47e392c8201a60d13ecf-Steve</t:Mailbox>
                     <t:SearchScope>All</t:SearchScope>
                  </t:MailboxSearchScope>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=f00c9f70539844beb52341d8f40c572e-Antho</t:Mailbox>
                     <t:SearchScope>PrimaryOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
            <t:MailboxQuery>
               <t:Query></t:Query>
               <t:MailboxSearchScopes>
                  <t:MailboxSearchScope>
                     <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=accba4fd5ddf12214a0e82ce1645f4e-Danie</t:Mailbox>
                     <t:SearchScope>ArchiveOnly</t:SearchScope>
                  </t:MailboxSearchScope>
               </t:MailboxSearchScopes>
            </t:MailboxQuery>
         </m:SearchQueries>
         <m:ResultType>StatisticsOnly</m:ResultType>
      </m:SearchMailboxes>
   </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [SearchMailboxes](searchmailboxes.md)
    
- [сеарчкуериес](searchqueries.md)
    
- [маилбокскуери](mailboxquery.md)
    
- [Query](query.md)
    
- [маилбокссеарчскопес](mailboxsearchscopes.md)
    
- [маилбокссеарчскопе](mailboxsearchscope.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [Тип](resulttype.md)
    
## <a name="successful-searchmailboxes-operation-response"></a>Успешный отклик операции SearchMailboxes

В следующем примере показан успешный ответ на запрос операции **SearchMailboxes** для получения статистической информации о количестве найденных терминов поиска в целевых почтовых ящиках. Последний запрос содержит пустой элемент **запроса** , в котором отображается неудачный Поиск в почтовом ящике. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=35181a94327e392c8201a60d13ecf-Steve</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                           <t:MailboxSearchScope>
                              <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=f00c9f789572-beb04001d8f40c572e-Antho</t:Mailbox>
                              <t:SearchScope>PrimaryOnly</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>2</t:ItemCount>
                  <t:Size>20206</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:KeywordStats>
                     <t:KeywordStat>
                        <t:Keyword>Test Item</t:Keyword>
                        <t:ItemHits>2</t:ItemHits>
                        <t:Size>20206</t:Size>
                     </t:KeywordStat>
                  </t:KeywordStats>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYPDLT)/cn=Recipients/cn=accba4as3df234234a0e82ce1645f4e-Danie</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>The search query can't be empty.</t:ErrorMessage>
                        <t:IsArchive>true</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Тело SOAP отклика содержит следующие элементы:
  
- [сеарчмаилбоксесреспонсе](searchmailboxesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [сеарчмаилбоксесреспонсемессаже](searchmailboxesresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [сеарчмаилбоксесресулт](searchmailboxesresult.md)
    
- [сеарчкуериес](searchqueries.md)
    
- [маилбокскуери](mailboxquery.md)
    
- [Query](query.md)
    
- [маилбокссеарчскопес](mailboxsearchscopes.md)
    
- [маилбокссеарчскопе](mailboxsearchscope.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [Тип](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [Размер (длинный)](size-long.md)
    
- [пажеитемкаунт](pageitemcount.md)
    
- [кэйвордстатс](keywordstats.md)
    
- [кэйвордстат](keywordstat.md)
    
- [Недопустим](keyword.md)
    
- [итемхитс](itemhits.md)
    
- [фаиледмаилбоксес](failedmailboxes.md)
    
- [фаиледмаилбокс](failedmailbox.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [ErrorCode (int)](errorcode-int.md)
    
- [ErrorMessage](errormessage.md)
    
- [IsArchive](isarchive.md)
    
## <a name="searchmailboxes-operation-error-response"></a>Ответ об ошибке операции SearchMailboxes

В следующем примере показан ответ об ошибке для запроса операции **SearchMailboxes** . Это ответ на запрос поиска в почтовом ящике при неправильном идентификаторе почтового ящика. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:SearchMailboxesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:SearchMailboxesResponseMessage ResponseClass="Error">
               <m:MessageText>No mailbox is specified for search operation. If specified in the request, 
               then it could be due to permission issue.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:SearchMailboxesResult>
                  <t:SearchQueries>
                     <t:MailboxQuery>
                        <t:Query>subject:Test Item</t:Query>
                        <t:MailboxSearchScopes>
                           <t:MailboxSearchScope>
                              <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                              <t:SearchScope>All</t:SearchScope>
                           </t:MailboxSearchScope>
                        </t:MailboxSearchScopes>
                     </t:MailboxQuery>
                  </t:SearchQueries>
                  <t:ResultType>StatisticsOnly</t:ResultType>
                  <t:ItemCount>0</t:ItemCount>
                  <t:Size>0</t:Size>
                  <t:PageItemCount>0</t:PageItemCount>
                  <t:PageItemSize>0</t:PageItemSize>
                  <t:FailedMailboxes>
                     <t:FailedMailbox>
                        <t:Mailbox>sbrown@contoso.com</t:Mailbox>
                        <t:ErrorCode>0</t:ErrorCode>
                        <t:ErrorMessage>No mailbox is specified for search operation. If specified in the request, 
                        then it could be due to permission issue.</t:ErrorMessage>
                        <t:IsArchive>false</t:IsArchive>
                     </t:FailedMailbox>
                  </t:FailedMailboxes>
               </m:SearchMailboxesResult>
            </m:SearchMailboxesResponseMessage>
         </m:ResponseMessages>
      </m:SearchMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [сеарчмаилбоксесреспонсе](searchmailboxesresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [сеарчмаилбоксесреспонсемессаже](searchmailboxesresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [сеарчмаилбоксесресулт](searchmailboxesresult.md)
    
- [сеарчкуериес](searchqueries.md)
    
- [маилбокскуери](mailboxquery.md)
    
- [Query](query.md)
    
- [маилбокссеарчскопес](mailboxsearchscopes.md)
    
- [маилбокссеарчскопе](mailboxsearchscope.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [SearchScope](searchscope.md)
    
- [Тип](resulttype.md)
    
- [ItemCount](itemcount.md)
    
- [Размер (длинный)](size-long.md)
    
- [пажеитемкаунт](pageitemcount.md)
    
- [пажеитемсизе](pageitemsize.md)
    
- [фаиледмаилбоксес](failedmailboxes.md)
    
- [фаиледмаилбокс](failedmailbox.md)
    
- [Mailbox (строка)](mailbox-string.md)
    
- [ErrorCode (int)](errorcode-int.md)
    
- [ErrorMessage](errormessage.md)
    
- [IsArchive](isarchive.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Операция SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Операция GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Операция GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Операция GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Операция GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

