---
title: Контакт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Элемент Contact представляет элемент контакта в Exchange магазине.
ms.openlocfilehash: a91d8cab7db0bfe0cc102aa75d51df5b60603a77
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543543"
---
# <a name="contact"></a>Контакт

Элемент **Contact** представляет элемент контакта в Exchange магазине. 
  
```XML
<Contact>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <Importance/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
   <FileAs/>
   <FileAsMapping/>
   <DisplayName/>
   <GivenName/>
   <Initials/>
   <MiddleName/>
   <Nickname/>
   <CompleteName/>
   <CompanyName/>
   <EmailAddresses/>
   <PhysicalAddresses/>
   <PhoneNumbers/>
   <AssistantName/>
   <Birthday/>
   <BusinessHomePage/>
   <Children/>
   <Companies/>
   <ContactSource/>
   <Department/>
   <Generation/>
   <ImAddresses/>
   <JobTitle/>
   <Manager/>
   <Mileage/>
   <OfficeLocation/>
   <PostalAddressIndex/>
   <Profession/>
   <SpouseName/>
   <Surname/>
   <WeddingAnniversary/>
   <HasPicture/>
   <PhoneticFullName/>
   <PhoneticFirstName/>
   <PhoneticLastName/>
   <Alias/>
   <Notes/>
   <Photo/>
   <UserSMIMECertificate/>
   <MSExchangeCertificate/>
   <DirectoryId/>
   <ManagerMailbox/>
   <DirectReports/>
</Contact>
```

 **ContactItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит родной многоцелевой поток расширения интернет-почты (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет субъект для Exchange элементов и объектов отклика.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень чувствительности элемента.  <br/> |
|[Основной текст](body.md) <br/> |Представляет фактическое содержимое тела сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время, когда элемент в почтовом ящике был получен.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в bytes элемента. Это свойство доступно только для чтения.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, которые определяют, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, на который этот элемент является ответом.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку по умолчанию "Избокс".  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет, был ли элемент еще не отправлен.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемент себе или себе.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, был ли элемент изменен.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заглавных сообщений в Интернете, содержащихся в элементе в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время, когда был отправлен элемент в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Этот элемент используется [элементом ReminderMinutesBeforeStart](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлено ли напоминание для элемента в Exchange магазине.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Представляет строку отображения, используемую для содержимого строки Cc. Это совмещенная строка всех имен отображения получателей Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Представляет строку отображения, используемую для содержимого строки To. Это конкаентированная строка всех имен отображения получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое настроено на **верное,** если элемент имеет хотя бы одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет культуру для данного элемента в почтовом ящике.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит имя отображения последнего пользователя, который должен изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает, когда элемент был изменен в последний раз.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для одновременного Microsoft Office Outlook конечной точки веб-приложения для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для одновременного Outlook Web App конечной точки для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или простой текст, который представляет уникальное тело этого разговора.  <br/> |
|[FileAs](fileas.md) <br/> |Представляет, как передается контакт в папке "Контакты".  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |Определяет, как создать то, что отображается для контакта.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Определяет имя отображения контакта.  <br/> |
|[GivenName](givenname.md) <br/> |Содержит имя контакта.  <br/> |
|[Initials](initials.md) <br/> |Представляет инициалы контакта.  <br/> |
|[MiddleName](middlename.md) <br/> |Представляет второе имя контакта.  <br/> |
|[Nickname](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[CompleteName](completename.md) <br/> |Представляет полное имя контакта.  <br/> |
|[CompanyName](companyname.md) <br/> |Представляет имя компании, связанное с контактом.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адресов электронной почты для контакта.  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |Содержит коллекцию физических адресов, связанных с контактом.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию номеров телефонов для контакта.  <br/> |
|[AssistantName](assistantname.md) <br/> |Представляет помощника для контакта.  <br/> |
|[Birthday](birthday.md) <br/> |Представляет дату рождения контакта.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Представляет домашняя страница (веб-адрес) для контакта.  <br/> |
|[Children](children.md) <br/> |Содержит имена детей контакта.  <br/> |
|[Companies](companies.md) <br/> |Представляет коллекцию компаний, связанных с контактом.  <br/> |
|[ContactSource](contactsource.md) <br/> |Описывает, находится ли контакт в Exchange магазине или службе каталога Active Directory.  <br/> |
|[Department](department.md) <br/> |Представляет отдел контакта на работе.  <br/> |
|[Generation](generation.md) <br/> |Представляет аббревиатура поколений, которая следует полному имени контакта.  <br/> |
|[ImAddresses](imaddresses.md) <br/> |Представляет коллекцию адресов обмена мгновенными сообщениями для контакта.  <br/> |
|[JobTitle](jobtitle.md) <br/> |Представляет название задания контакта.  <br/> |
|[Сотрудник](manager.md) <br/> |Представляет диспетчер контакта.  <br/> |
|[Mileage](mileage.md) <br/> |Представляет пробег для контактного элемента.  <br/> |
|[OfficeLocation](officelocation.md) <br/> |Представляет расположение контакта в офисе.  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |Представляет типы отображения для физических адресов.  <br/> |
|[Profession](profession.md) <br/> |Представляет профессию контакта.  <br/> |
|[Имя spouseName](spousename.md) <br/> |Представляет имя супруга или партнера контакта.  <br/> |
|[Фамилия](surname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |Содержит годовщину свадьбы контакта.  <br/> |
|[HasPicture](haspicture.md) <br/> |Указывает, есть ли у контактного элемента вложение файла, представляю которое представляет изображение контакта.  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |Содержит полное имя контакта, включая имя и фамилию, написанное фонетически.  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |Содержит имя контакта, написанное фонетически.  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |Содержит фамилию контакта, написанную фонетически.  <br/> |
|[Alias](alias.md) <br/> |Содержит псевдоним электронной почты контакта.  <br/> |
|[Notes (Contact)](notes-contact.md) <br/> |Содержит дополнительные контактные данные.  <br/> |
|[Фотография](photo.md) <br/> |Содержит значение, кодирует фотографию контакта.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Содержит значение, кодированное сертификатом SMIME контакта.  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |Содержит значение, которое кодирует сертификат microsoft Exchange контакта.  <br/> |
|[DirectoryId](directoryid.md) <br/> |Содержит ИД каталога контакта.  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |Содержит сведения SMTP, которые идентифицируют почтовый ящик диспетчера контакта.  <br/> |
|[DirectReports](directreports.md) <br/> |Содержит сведения SMTP, определяя прямые отчеты контакта.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описывает все элементы календаря, которые примыкают к времени собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Определяет данные для приложения к одному свойству элемента или папки во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуются со временем собрания  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Определяет одну папку, создаемую в локальном клиентской магазине.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, идентифицированной элементом [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[Решение](resolution.md) <br/> |Содержит одну разрешенную сущность.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном клиентской магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание контактов (Exchange веб-служб)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Удаление контактов](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

