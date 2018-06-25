---
title: Контакт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contact
api_type:
- schema
ms.assetid: 66bfff50-7a91-4d81-b6a0-610b9962f677
description: Элемент контакта представляет элемента контакта в хранилище Exchange.
ms.openlocfilehash: 7b2e7c0197914c2a0a0ba3815dd05fca52a5f872
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761731"
---
# <a name="contact"></a>Контакт

Элемент **контактов** представляет элемента контакта в хранилище Exchange. 
  
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
|[MimeContent](mimecontent.md) <br/> |Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Subject](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объекты ответа.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Указывает уровень конфиденциальности для элемента.  <br/> |
|[Body](body.md) <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах элемента. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, к которому этот элемент является ее в ответ.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, является ли элемент был отправлен исходящие папке по умолчанию.  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет ли элемент еще не были отправлены.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Показывает пользователя отправить элемент в себе.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, является ли элемент ранее еще был отправлен.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, были ли изменены элемента.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлен ли напоминания для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет число минут и только потом событие, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Строка отображения, который используется для содержимого строку "Копия". Это составное строка всех получателей отображаемые имена «копия».  <br/> |
|[DisplayTo](displayto.md) <br/> |Строка отображения, который используется для содержимого строке. Это составное строка всех для получателей отображаемые имена.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Язык и региональные параметры](culture.md) <br/> |Представляет язык и региональные параметры для заданного элемента в почтовом ящике.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, является ли элемент связан с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.  <br/> |
|[FileAs](fileas.md) <br/> |Представляет, как оформлена контакт в папке «Контакты».  <br/> |
|[FileAsMapping](fileasmapping.md) <br/> |Определяет порядок создания, отображаемых для контакта.  <br/> |
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Задает отображаемое имя контакта.  <br/> |
|[GivenName](givenname.md) <br/> |Содержит имя контакта.  <br/> |
|[Инициалы](initials.md) <br/> |Представляет отчество контакта.  <br/> |
|[Отчество](middlename.md) <br/> |Представляет отчество контакта.  <br/> |
|[Понятное имя](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[CompleteName](completename.md) <br/> |Представляет полное имя контакта.  <br/> |
|[Название организации](companyname.md) <br/> |Представляет имя компании, связанное с контактом.  <br/> |
|[EmailAddresses](emailaddresses.md) <br/> |Представляет коллекцию адреса электронной почты контакта.  <br/> |
|[PhysicalAddresses](physicaladdresses.md) <br/> |Содержит коллекцию физических адресов, связанные с контактом.  <br/> |
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию телефонных номеров контакта.  <br/> |
|[AssistantName](assistantname.md) <br/> |Представляет помощника контакта.  <br/> |
|[День рождения](birthday.md) <br/> |Представляет Дата рождения контакта.  <br/> |
|[BusinessHomePage](businesshomepage.md) <br/> |Представляет Домашняя страница (веб-адрес) для этого контакта.  <br/> |
|[Дочерние элементы](children.md) <br/> |Содержит имена дочерних элементов контакта.  <br/> |
|[Компании](companies.md) <br/> |Представляет коллекцию компании, связанные с контактом.  <br/> |
|[ContactSource](contactsource.md) <br/> |Описание, находится ли контакт в хранилище Exchange или службе каталогов Active Directory.  <br/> |
|[Отдел](department.md) <br/> |Представляет отдел контакта на работе.  <br/> |
|[Создание](generation.md) <br/> |Представляет поколениям аббревиатура, исходя из полного имени контакта.  <br/> |
|[ImAddresses](imaddresses.md) <br/> |Представляет коллекцию мгновенного обмена сообщениями адресов для контакта.  <br/> |
|[Название должности](jobtitle.md) <br/> |Представляет должность контакта.  <br/> |
|[Руководитель](manager.md) <br/> |Представляет диспетчера контактов.  <br/> |
|[Расстояние](mileage.md) <br/> |Представляет расстояние для элемента контакта.  <br/> |
|[Расположение компании](officelocation.md) <br/> |Представляет расположение комнаты контакта.  <br/> |
|[PostalAddressIndex](postaladdressindex.md) <br/> |Представляет типов отображения физических адресов.  <br/> |
|[Род занятий](profession.md) <br/> |Представляет род занятий контакта.  <br/> |
|[SpouseName](spousename.md) <br/> |Представляет имя контакта супруга/партнера.  <br/> |
|[Фамилия](surname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[WeddingAnniversary](weddinganniversary.md) <br/> |Содержит Годовщина свадьбы контакта.  <br/> |
|[HasPicture](haspicture.md) <br/> |Указывает, имеет ли элемент контактов вложенный файл, который представляет на изображение контакта.  <br/> |
|[PhoneticFullName](phoneticfullname.md) <br/> |Содержит полное имя контакта, включая имя и фамилию, фонетически.  <br/> |
|[PhoneticFirstName](phoneticfirstname.md) <br/> |Содержит имя контакта, фонетически.  <br/> |
|[PhoneticLastName](phoneticlastname.md) <br/> |Содержит фамилию контакта, фонетически.  <br/> |
|[Псевдоним](alias.md) <br/> |Содержит псевдоним электронной почты контакта.  <br/> |
|[Примечания (контактов)](notes-contact.md) <br/> |Содержит дополнительные контактные сведения.  <br/> |
|[Photo](photo.md) <br/> |Содержит значение, которое кодирует фотографии контакта.  <br/> |
|[UserSMIMECertificate](usersmimecertificate.md) <br/> |Содержит значение, которое кодирует сертификат SMIME контакта.  <br/> |
|[MSExchangeCertificate](msexchangecertificate.md) <br/> |Содержит значение, которое кодирует сертификата Microsoft Exchange контакта.  <br/> |
|[DirectoryId](directoryid.md) <br/> |Содержит идентификатор каталога контакта.  <br/> |
|[ManagerMailbox](managermailbox.md) <br/> |Содержит сведения SMTP, который идентифицирует почтовый ящик диспетчера контакта.  <br/> |
|[DirectReports](directreports.md) <br/> |Содержит SMTP идентификационные сведения о прямых отчетов контакта.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания  <br/> |
|[Создание (ItemSync)](create-itemsync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[Элементы](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[Решение](resolution.md) <br/> |Содержит одного объекта разрешения.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[Обновление (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Создание контактов (веб-служб Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)
  
[Обновление контактов](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Удаление контактов](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

