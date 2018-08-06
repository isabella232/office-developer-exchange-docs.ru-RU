---
title: Начало работы с клиентскими приложениями EWS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Создание первого приложения с помощью веб-служб Exchange (EWS) в Exchange.
ms.openlocfilehash: 06606bdc2b37c8bf65b8b10dc7a516bdc911b256
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353779"
---
# <a name="get-started-with-ews-client-applications"></a>Начало работы с клиентскими приложениями EWS

Создание первого приложения с помощью веб-служб Exchange (EWS) в Exchange.
  
EWS  это комплексная служба, которую приложения могут использовать для получения доступа практически ко всем данным, хранящимся в почтовом ящике локальной версии Exchange, Exchange Online или Exchange Online в составе Office 365. Для обеспечения доступа к серверу Exchange Server служба EWS использует стандартные веб-протоколы. Такие библиотеки, как [EWS Managed API](get-started-with-ews-managed-api-client-applications.md), позволяют преобразовать операции EWS для предоставления объектно-ориентированного интерфейса. Ознакомившись с примерами в этой статье, вы получите некоторое понимание того, что можно делать с помощью EWS. 
  
Операции EWS можно вызвать из любой операционной системы и с помощью любого языка, потому что при обработке запросов и откликов EWS используется протокол SOAP. Примеры в этой статье написаны на языке C# с использованием объектов [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) и [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) .NET Framework. Но важная составляющая кода  это XML-код, который используется для создания запросов EWS и возврата XML-откликов с сервера. В примерах кода основное внимание уделяется XML-транзакциям, а не обработке XML. 
  
## <a name="youll-need-an-exchange-server"></a>Вам потребуется сервер Exchange Server

Если у вас уже есть учетная запись почтового ящика Exchange, вы можете пропустить этот шаг. Если это не так, ниже приведены несколько вариантов настройки почтового ящика Exchange для вашего первого приложения EWS.
  
- [Создайте Сайт разработчика в Office 365](http://msdn.microsoft.com/ru-RU/library/office/fp179924.aspx) (рекомендуется). Так можно получить почтовый ящик Exchange быстрее всего.
    
- Скачайте [Exchange Server](http://office.microsoft.com/en-us/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).
    
Когда вы проверите, можно ли отправлять сообщения на сервер Exchange Server и получать их с него, приступайте к настройке среды разработки. Проверить отправку сообщений можно с помощью Outlook Web App.
  
Необходимо знать URL-адрес конечной точки EWS для сервера. Для определения этого URL-адреса в рабочем приложении используйте функцию [автообнаружения](autodiscover-for-exchange.md). В примерах из этой статьи используется URL-адрес конечной точки EWS в Office 365 (`https://outlook.office365.com/EWS/Exchange.asmx`. Ссылки на дополнительные сведения о функции автообнаружения можно найти в разделе [Дальнейшие действия](#bk_next). 
  
Если вы будете тестировать приложение на сервере Exchange Server, который использует самозаверяющий сертификат по умолчанию, вам потребуется создать [метод проверки сертификата](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) в соответствии с требованиями вашей организации к обеспечению безопасности. 
  
## <a name="set-up-your-development-environment"></a>Настройка среды разработки

Выбор инструментов для создания вашего первого приложения EWS зависит от операционной системы и языка, которые вы используете, но в основном это дело вкуса. Если вы хотите воспользоваться примерами на языке C# из этой статьи, вам понадобится следующее: 
  
- Любая версия Visual Studio, поддерживающая .NET Framework 4.0. 
    
- Подключение к Интернету, необходимое для связи компьютера для разработки с сервером Exchange Server. Если вы можете использовать Outlook Web App и DNS-имя вместо IP-адреса для соединения с сервером Exchange Server, все настроено.
    
## <a name="create-your-first-ews-application"></a>Создание первого приложения EWS

Созданное приложение EWS продемонстрирует два стандартных сценария использования EWS:
  
1. Получение данных из почтового ящика Exchange и предоставление их пользователю.
    
2. Выполнение какого-либо действия (например, отправки электронного сообщения) и проверка отклика для подтверждения успешного завершения.
    
Теперь можно приступать к работе.
  
### <a name="set-up-the-solution"></a>Настройка решения

Сначала необходимо создать новое консольное приложение с помощью Visual Studio, а затем — новый объект под названием Tracing.cs. Этот объект используется для записи информации в файлы журнала и консоли, чтобы после запуска кода отобразились результаты. Вставьте в файл Tracing.cs указанный ниже код.
  
```cs
using System;
using System.IO;
namespace Microsoft.Exchange.Samples.EWS
{
  class Tracing
  {
    private static TextWriter logFileWriter = null;
    public static void OpenLog(string fileName)
    {
      logFileWriter = new StreamWriter(fileName);
    }
    public static void Write(string format, params object[] args)
    {
      Console.Write(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.Write(format, args);
      }
    }
    public static void WriteLine(string format, params object[] args)
    {
      Console.WriteLine(format, args);
      if (logFileWriter != null)
      {
        logFileWriter.WriteLine(format, args);
      }
    }
    public static void CloseLog()
    {
      logFileWriter.Flush();
      logFileWriter.Close();
    }
  }
}
```

Затем откройте файл Program.cs. В него будет помещена оставшаяся часть кода, используемого в качестве примера.
  
Сначала необходимо настроить программную оболочку. Программа выполнит следующее: 
  
1. Создаст файл журнала для записи на диск запросов и откликов, чтобы позже их можно было изучить.
    
2. Получит доступ к электронному адресу и паролю учетной записи, которые вы будете использовать.
    
3. Вызовет примеры методов.
    
Замените метод  `Main` в файле Program.cs указанным ниже кодом. 
  
```cs
    static void Main(string[] args)
    {
      // Start tracing to console and a log file.
      Tracing.OpenLog("./GetStartedWithEWS.log");
      Tracing.WriteLine("EWS sample application started.");
      var isValidEmailAddress = false;
      Console.Write("Enter an email address: ");
      var emailAddress = Console.ReadLine();
      
        isValidEmailAddress = (emailAddress.Contains("@") &amp;&amp; emailAddress.Contains("."));
      if (!isValidEmailAddress)
      {
        Tracing.WriteLine("Email address " + emailAddress + " is not a valid SMTP address. Closing program.");
        return;
      }
      SecureString password = GetPasswordFromConsole();
      if (password.Length == 0)
      {
        Tracing.WriteLine("Password empty, closing program.");
      }
      NetworkCredential userCredentials = new NetworkCredential(emailAddress, password);
      // These are the sample methods that demonstrate using EWS.
      // ShowNumberOfMessagesInInbox(userCredentials);
      // SendTestEmail(userCredentials);
     
      Tracing.WriteLine("EWS sample application ends.");
      Tracing.CloseLog();
      Console.WriteLine("Press enter to exit: ");
      Console.ReadLine();
    }
    // These method stubs will be filled in later.
    private static void ShowNumberOfMessagesInInbox(NetworkCredential userCredentials)
    {
    }
    private static void SendTestEmail(NetworkCredential userCredentials)
    {
    }
```

Напоследок вам необходимо добавить статический метод  `GetPasswordFromConsole`. Этот метод возвращает объект [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) , содержащий введенный в консоль пароль. 
  
```cs
    private static SecureString GetPasswordFromConsole()
    {
      SecureString password = new SecureString();
      bool readingPassword = true;
      Console.Write("Enter password: ");
      while (readingPassword)
      {
        ConsoleKeyInfo userInput = Console.ReadKey(true);
        switch (userInput.Key)
        {
          case (ConsoleKey.Enter):
            readingPassword = false;
            break;
          case (ConsoleKey.Escape):
            password.Clear();
            readingPassword = false;
            break;
          case (ConsoleKey.Backspace):
            if (password.Length > 0)
            {
              password.RemoveAt(password.Length - 1);
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
              Console.Write(" ");
              Console.SetCursorPosition(Console.CursorLeft - 1, Console.CursorTop);
            }
            break;
          default:
            if (userInput.KeyChar != 0)
            {
              password.AppendChar(userInput.KeyChar);
              Console.Write("*");
            }
            break;
        }
      }
      Console.WriteLine();
      password.MakeReadOnly();
      return password;
    }
```

### <a name="get-the-number-of-new-messages-in-an-inbox"></a>Число новых сообщений в папке "Входящие"

Получение сведений об электронных сообщениях, собраниях, встречах, а также папках, в которых эти сведения хранятся,  типовые операции в приложении EWS. Этот пример поможет узнать, сколько сообщений находится в папке "Входящие" учетной записи, а также общее число сообщений и число непрочитанных сообщений. Пример демонстрирует следующие типовые действия для приложений EWS:
  
- отправка запроса EWS на сервер Exchange;
    
- анализ возвращенного XML-отклика на наличие запрошенной информации;
    
- обработка типовых исключений и сообщений об ошибке.
    
Добавьте указанный ниже код в метод  `ShowNumberOfMessagesInInbox`, заглушенный вслед за основным. При запуске приложения будет показано число непрочитанных сообщений и число сообщений в папке "Входящие" учетной записи. Запустив приложение, вы сможете открыть файл GetStartedWithEWS.log и просмотреть XML-запрос, отправленный на сервер Exchange Server, и возвращенный сервером отклик. 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"      <FolderShape>\n" +
"        <t:BaseShape>Default</t:BaseShape>\n" +
"      </FolderShape>\n" +
"      <FolderIds>\n" +
"        <t:DistinguishedFolderId Id=\"inbox\"/>\n" +
"      </FolderIds>\n" +
"    </GetFolder>\n" +
"  </soap:Body>\n" +
"</soap:Envelope>\n";
      // Write the get folder operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(getFolderSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(getFolderSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            // Process the response.
            IEnumerable<XElement> folders = from folderElement in
                                              responseEnvelope.Descendants
                                              ("{http://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{http://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{http://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
                               select folderElement.Value;
              Tracing.WriteLine(unreadCount.ElementAt(0));
            }
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }

```

### <a name="send-an-email-message"></a>Отправка электронных сообщений

Отправка электронных сообщений или приглашений на собрания — это еще одна типовая операция приложения EWS. Данный пример позволяет создать и отправить сообщение с помощью введенных ранее учетных данных пользователя. Пример демонстрирует следующие типовые задачи приложений EWS:
  
- создание и отправка электронных сообщений;
    
- анализ возвращенного XML-отклика для определения того, было ли сообщение отправлено корректно;
    
- обработка типовых исключений и сообщений об ошибке.
    
Добавьте указанный ниже код в метод SendTestEmail, заглушенный вслед за основным. Запустив приложение, вы можете открыть файл GetStartedWithEWS.log и просмотреть XML-запрос, отправленный на сервер Exchange Server, и возвращенный сервером отклик.
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\">\n" +
      "  <soap:Header>\n" +
      "    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
      "  </soap:Header>\n" +
      "  <soap:Body>\n" +
      "    <m:CreateItem MessageDisposition=\"SendAndSaveCopy\">\n" +
      "      <m:SavedItemFolderId>\n" +
      "        <t:DistinguishedFolderId Id=\"sentitems\" />\n" +
      "      </m:SavedItemFolderId>\n" +
      "      <m:Items>\n" +
      "        <t:Message>\n" +
      "          <t:Subject>Company Soccer Team</t:Subject>\n" +
      "          <t:Body BodyType=\"HTML\">Are you interested in joining?</t:Body>\n" +
      "          <t:ToRecipients>\n" +
      "            <t:Mailbox>\n" +
      "              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>\n" +
      "              </t:Mailbox>\n" +
      "          </t:ToRecipients>\n" +
      "        </t:Message>\n" +
      "      </m:Items>\n" +
      "    </m:CreateItem>\n" +
      "  </soap:Body>\n" +
      "</soap:Envelope>\n";
      // Write the create item operation request to the console and log file.
      Tracing.WriteLine("Get folder operation request:");
      Tracing.WriteLine(createItemSOAPRequest);
      var getFolderRequest = WebRequest.CreateHttp(Office365WebServicesURL);
      getFolderRequest.AllowAutoRedirect = false;
      getFolderRequest.Credentials = userCredentials;
      getFolderRequest.Method = "POST";
      getFolderRequest.ContentType = "text/xml";
      var requestWriter = new StreamWriter(getFolderRequest.GetRequestStream());
      requestWriter.Write(createItemSOAPRequest);
      requestWriter.Close();
      try
      {
        var getFolderResponse = (HttpWebResponse)(getFolderRequest.GetResponse());
        if (getFolderResponse.StatusCode == HttpStatusCode.OK)
        {
          var responseStream = getFolderResponse.GetResponseStream();
          XElement responseEnvelope = XElement.Load(responseStream);
          if (responseEnvelope != null)
          {
            // Write the response to the console and log file.
            Tracing.WriteLine("Response:");
            StringBuilder stringBuilder = new StringBuilder();
            XmlWriterSettings settings = new XmlWriterSettings();
            settings.Indent = true;
            XmlWriter writer = XmlWriter.Create(stringBuilder, settings);
            responseEnvelope.Save(writer);
            writer.Close();
            Tracing.WriteLine(stringBuilder.ToString());
            // Check the response for error codes. If there is an error, throw an application exception.
            IEnumerable<XElement> errorCodes = from errorCode in responseEnvelope.Descendants
                                               ("{http://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
                                               select errorCode;
            foreach (var errorCode in errorCodes)
            {
              if (errorCode.Value != "NoError")
              {
                switch (errorCode.Parent.Name.LocalName.ToString())
                {
                  case "Response":
                    string responseError = "Response-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(responseError);
                  case "UserResponse":
                    string userError = "User-level error getting inbox information:\n" + errorCode.Value;
                    throw new ApplicationException(userError);
                }
              }
            }
            Tracing.WriteLine("Message sent successfully.");
          }
        }
      }
      catch (WebException ex)
      {
        Tracing.WriteLine("Caught Web exception:");
        Tracing.WriteLine(ex.Message);
      }
      catch (ApplicationException ex)
      {
        Tracing.WriteLine("Caught application exception:");
        Tracing.WriteLine(ex.Message);
      }
```

<a name="bk_next"></a>

## <a name="next-steps"></a>Дальнейшие действия

Теперь, когда вы написали свое первое приложение EWS, можно переходить к другим способам использования EWS. Вот несколько идей для начала работы:
  
- Реализуйте в приложении функции [автообнаружения](autodiscover-for-exchange.md), чтобы оно могло соединиться с нужным сервером Exchange Server, используя электронный адрес пользователя. См. также пример в статье [Exchange 2013: получение параметров пользователей с помощью автообнаружения](http://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e). 
    
- Ознакомьтесь со [справкой по EWS](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) для получения дополнительных сведений об EWS. 
    
- Просмотрите список [операций EWS](http://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) для получения сведений о доступных операциях. 
    
- Используйте [редактор EWS](http://ewseditor.codeplex.com/) для просмотра траффика SOAP, отправляемого на сервер и обратно. 
    
Если с приложением возникли проблемы, [попробуйте опубликовать вопрос или комментарий на форуме](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) (и не забудьте прочитать первую запись). 
  
## <a name="see-also"></a>См. также

- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)   
- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)  
- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md)
    

