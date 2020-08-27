---
title: Начало работы с клиентскими приложениями EWS
manager: sethgros
ms.date: 8/26/2020
ms.audience: Developer
ms.assetid: e6fd5c23-0ba5-4a7b-bdde-4a553447069f
description: Создание первого приложения с помощью веб-служб Exchange (EWS) в Exchange.
localization_priority: Priority
ms.openlocfilehash: 81d4cb69d20f17945658ab4ad16c9fe3a47d4eec
ms.sourcegitcommit: 636c05a929279812c6ef87d75b01c166a4a05584
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/26/2020
ms.locfileid: "47254981"
---
# <a name="get-started-with-ews-client-applications"></a><span data-ttu-id="64355-103">Начало работы с клиентскими приложениями EWS</span><span class="sxs-lookup"><span data-stu-id="64355-103">Get started with EWS client applications</span></span>

<span data-ttu-id="64355-104">Создание первого приложения с помощью веб-служб Exchange (EWS) в Exchange.</span><span class="sxs-lookup"><span data-stu-id="64355-104">Create your first application by using Exchange Web Services (EWS) in Exchange.</span></span>
  
<span data-ttu-id="64355-p101">EWS  это комплексная служба, которую приложения могут использовать для получения доступа практически ко всем данным, хранящимся в почтовом ящике локальной версии Exchange, Exchange Online или Exchange Online в составе Office 365. Для обеспечения доступа к серверу Exchange Server служба EWS использует стандартные веб-протоколы. Такие библиотеки, как [EWS Managed API](get-started-with-ews-managed-api-client-applications.md), позволяют преобразовать операции EWS для предоставления объектно-ориентированного интерфейса. Ознакомившись с примерами в этой статье, вы получите некоторое понимание того, что можно делать с помощью EWS.</span><span class="sxs-lookup"><span data-stu-id="64355-p101">EWS is a comprehensive service that your applications can use to access almost all the information stored in an Exchange Online, Exchange Online as part of Office 365, or Exchange on-premises mailbox. EWS uses standard web protocols to provide access to an Exchange server; libraries like the [EWS Managed API](get-started-with-ews-managed-api-client-applications.md) wrap the EWS operations to provide an object-oriented interface. After you've run the examples in this article, you will have a basic understanding of what you can do with EWS.</span></span> 
  
<span data-ttu-id="64355-p102">Операции EWS можно вызвать из любой операционной системы и с помощью любого языка, потому что при обработке запросов и откликов EWS используется протокол SOAP. Примеры в этой статье написаны на языке C# с использованием объектов [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) и [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) .NET Framework. Но важная составляющая кода  это XML-код, который используется для создания запросов EWS и возврата XML-откликов с сервера. В примерах кода основное внимание уделяется XML-транзакциям, а не обработке XML.</span><span class="sxs-lookup"><span data-stu-id="64355-p102">You can call EWS operations from any operating system or language, because the EWS requests and responses use the SOAP protocol. The examples in this article are written using C# and make use of the .NET Framework [HttpWebRequest](https://msdn.microsoft.com/library/System.Net.HttpWebRequest.aspx) and [HttpWebResponse](https://msdn.microsoft.com/library/System.Net.HttpWebResponse.aspx) objects; however, the important part of the code is the XML used to make the EWS request and the XML response returned from the server. The code examples emphasize the XML transactions and not processing the XML.</span></span> 
  
## <a name="youll-need-an-exchange-server"></a><span data-ttu-id="64355-111">Вам потребуется сервер Exchange Server</span><span class="sxs-lookup"><span data-stu-id="64355-111">You'll need an Exchange server</span></span>

<span data-ttu-id="64355-p103">Если у вас уже есть учетная запись почтового ящика Exchange, вы можете пропустить этот шаг. Если это не так, ниже приведены несколько вариантов настройки почтового ящика Exchange для вашего первого приложения EWS.</span><span class="sxs-lookup"><span data-stu-id="64355-p103">If you already have an Exchange mailbox account, you can skip this step. Otherwise, you have the following options for setting up an Exchange mailbox for your first EWS application:</span></span>
  
- <span data-ttu-id="64355-p104">[Создайте Сайт разработчика в Office 365](https://developer.microsoft.com/microsoft-365/dev-program) (рекомендуется). Так можно получить почтовый ящик Exchange быстрее всего.</span><span class="sxs-lookup"><span data-stu-id="64355-p104">[Get an Office 365 Developer Site ](https://developer.microsoft.com/microsoft-365/dev-program)(recommended). This is the quickest way for you to get an Exchange mailbox.</span></span>
    
- <span data-ttu-id="64355-116">Скачайте [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span><span class="sxs-lookup"><span data-stu-id="64355-116">Download [Exchange Server](https://office.microsoft.com/exchange/microsoft-exchange-try-or-buy-exchange-we-can-help-you-decide-FX103746846.aspx?WT%2Eintid1=ODC%5FENUS%5FFX103472230%5FXT103965589).</span></span>

    
<span data-ttu-id="64355-p105">Когда вы проверите, можно ли отправлять сообщения на сервер Exchange Server и получать их с него, приступайте к настройке среды разработки. Проверить отправку сообщений можно с помощью Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="64355-p105">After you've verified that you can send and receive email from your Exchange server you are ready to set up your development environment. You can use Outlook Web App to verify that you can send email.</span></span>
  
<span data-ttu-id="64355-p106">Необходимо знать URL-адрес конечной точки EWS для сервера. Для определения этого URL-адреса в рабочем приложении используйте функцию [автообнаружения](autodiscover-for-exchange.md). В примерах из этой статьи используется URL-адрес конечной точки EWS в Office 365 (`https://outlook.office365.com/EWS/Exchange.asmx`. Ссылки на дополнительные сведения о функции автообнаружения можно найти в разделе [Дальнейшие действия](#bk_next).</span><span class="sxs-lookup"><span data-stu-id="64355-p106">You'll also need to know the URL of the EWS endpoint for your server. In a production application, you'd use [Autodiscover](autodiscover-for-exchange.md) to determine the EWS URL. The examples in this article use the Office 365 EWS endpoint URL, `https://outlook.office365.com/EWS/Exchange.asmx`. The [Next steps](#bk_next) section has links to more information about Autodiscover when you're ready.</span></span> 
  
<span data-ttu-id="64355-123">Если вы будете тестировать приложение на сервере Exchange Server, который использует самозаверяющий сертификат по умолчанию, вам потребуется создать [метод проверки сертификата](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) в соответствии с требованиями вашей организации к обеспечению безопасности.</span><span class="sxs-lookup"><span data-stu-id="64355-123">If you are testing your application using an Exchange server that has the default self-signed certificate, you'll need to create a [certificate validation method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md) that meets the security requirements of your organization.</span></span> 
  
## <a name="set-up-your-development-environment"></a><span data-ttu-id="64355-124">Настройка среды разработки</span><span class="sxs-lookup"><span data-stu-id="64355-124">Set up your development environment</span></span>

<span data-ttu-id="64355-p107">Выбор инструментов для создания вашего первого приложения EWS зависит от операционной системы и языка, которые вы используете, но в основном это дело вкуса. Если вы хотите воспользоваться примерами на языке C# из этой статьи, вам понадобится следующее:</span><span class="sxs-lookup"><span data-stu-id="64355-p107">The tools that you use to create your first EWS application depend on the operating system and language that you use, and are mostly a matter of taste. If you want to follow along with the C# examples in this article, you'll need:</span></span> 
  
- <span data-ttu-id="64355-127">Любая версия Visual Studio, поддерживающая .NET Framework 4.0.</span><span class="sxs-lookup"><span data-stu-id="64355-127">Any version of Visual Studio that supports the .NET Framework 4.0.</span></span> 
    
- <span data-ttu-id="64355-p108">Подключение к Интернету, необходимое для связи компьютера для разработки с сервером Exchange Server. Если вы можете использовать Outlook Web App и DNS-имя вместо IP-адреса для соединения с сервером Exchange Server, все настроено.</span><span class="sxs-lookup"><span data-stu-id="64355-p108">An Internet connection that your development machine can use to contact your Exchange server. If you can use Outlook Web App with a DNS name rather than an IP address to connect to your Exchange server, you are set up.</span></span>
    
## <a name="create-your-first-ews-application"></a><span data-ttu-id="64355-130">Создание первого приложения EWS</span><span class="sxs-lookup"><span data-stu-id="64355-130">Create your first EWS application</span></span>

<span data-ttu-id="64355-131">Созданное приложение EWS продемонстрирует два стандартных сценария использования EWS:</span><span class="sxs-lookup"><span data-stu-id="64355-131">The EWS application that you will create shows two typical scenarios for using EWS:</span></span>
  
1. <span data-ttu-id="64355-132">Получение данных из почтового ящика Exchange и предоставление их пользователю.</span><span class="sxs-lookup"><span data-stu-id="64355-132">Get information from an Exchange mailbox and display that information to the user.</span></span>
    
2. <span data-ttu-id="64355-133">Выполнение какого-либо действия (например, отправки электронного сообщения) и проверка отклика для подтверждения успешного завершения.</span><span class="sxs-lookup"><span data-stu-id="64355-133">Perform an action, such as sending an email, and check the response to see if the action succeeded.</span></span>
    
<span data-ttu-id="64355-134">Теперь можно приступать к работе.</span><span class="sxs-lookup"><span data-stu-id="64355-134">Let's get started.</span></span>
  
### <a name="set-up-the-solution"></a><span data-ttu-id="64355-135">Настройка решения</span><span class="sxs-lookup"><span data-stu-id="64355-135">Set up the solution</span></span>

<span data-ttu-id="64355-p109">Сначала необходимо создать новое консольное приложение с помощью Visual Studio, а затем — новый объект под названием Tracing.cs. Этот объект используется для записи информации в файлы журнала и консоли, чтобы после запуска кода отобразились результаты. Вставьте в файл Tracing.cs указанный ниже код.</span><span class="sxs-lookup"><span data-stu-id="64355-p109">First, create a new console application solution using Visual Studio. When the solution is ready, create a new object called Tracing.cs. Use this object to write information to both the console and a log file so that you can review the results after you run your code. Paste the following code into the Tracing.cs file.</span></span>
  
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

<span data-ttu-id="64355-p110">Затем откройте файл Program.cs. В него будет помещена оставшаяся часть кода, используемого в качестве примера.</span><span class="sxs-lookup"><span data-stu-id="64355-p110">Next, open the Program.cs file. You will put the rest of the code for the example in this file.</span></span>
  
<span data-ttu-id="64355-p111">Сначала необходимо настроить программную оболочку. Программа выполнит следующее:</span><span class="sxs-lookup"><span data-stu-id="64355-p111">First, set up the shell of the program. The program will:</span></span> 
  
1. <span data-ttu-id="64355-144">Создаст файл журнала для записи на диск запросов и откликов, чтобы позже их можно было изучить.</span><span class="sxs-lookup"><span data-stu-id="64355-144">Create a log file so that the request and response can be written to disk for later study.</span></span>
    
2. <span data-ttu-id="64355-145">Получит доступ к электронному адресу и паролю учетной записи, которые вы будете использовать.</span><span class="sxs-lookup"><span data-stu-id="64355-145">Get the email address and password of the account that you'll access.</span></span>
    
3. <span data-ttu-id="64355-146">Вызовет примеры методов.</span><span class="sxs-lookup"><span data-stu-id="64355-146">Call the sample methods.</span></span>
    
<span data-ttu-id="64355-147">Замените метод  `Main` в файле Program.cs указанным ниже кодом.</span><span class="sxs-lookup"><span data-stu-id="64355-147">Replace the  `Main` method in the Program.cs with the following code.</span></span> 
  
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

<span data-ttu-id="64355-p112">Напоследок вам необходимо добавить статический метод  `GetPasswordFromConsole`. Этот метод возвращает объект [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) , содержащий введенный в консоль пароль.</span><span class="sxs-lookup"><span data-stu-id="64355-p112">The last thing that you need to do is add the  `GetPasswordFromConsole` static method. This method returns a [SecureString](https://msdn.microsoft.com/library/System.Security.SecureString.aspx) object that contains a password typed at the console.</span></span> 
  
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

### <a name="get-the-number-of-new-messages-in-an-inbox"></a><span data-ttu-id="64355-150">Число новых сообщений в папке "Входящие"</span><span class="sxs-lookup"><span data-stu-id="64355-150">Get the number of new messages in an Inbox</span></span>

<span data-ttu-id="64355-p113">Получение сведений об электронных сообщениях, собраниях, встречах, а также папках, в которых эти сведения хранятся,  типовые операции в приложении EWS. Этот пример поможет узнать, сколько сообщений находится в папке "Входящие" учетной записи, а также общее число сообщений и число непрочитанных сообщений. Пример демонстрирует следующие типовые действия для приложений EWS:</span><span class="sxs-lookup"><span data-stu-id="64355-p113">A common operation in an EWS application is to get information about email messages, appointments, meetings, and the folders that store them. This example gets the number of messages in an account's Inbox and displays the total number of messages and the number of unread messages. It demonstrates the following common actions for EWS applications:</span></span>
  
- <span data-ttu-id="64355-154">отправка запроса EWS на сервер Exchange;</span><span class="sxs-lookup"><span data-stu-id="64355-154">Making an EWS request to the Exchange server.</span></span>
    
- <span data-ttu-id="64355-155">анализ возвращенного XML-отклика на наличие запрошенной информации;</span><span class="sxs-lookup"><span data-stu-id="64355-155">Parsing the returned XML response for the requested information.</span></span>
    
- <span data-ttu-id="64355-156">обработка типовых исключений и сообщений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="64355-156">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="64355-p114">Добавьте указанный ниже код в метод  `ShowNumberOfMessagesInInbox`, заглушенный вслед за основным. При запуске приложения будет показано число непрочитанных сообщений и число сообщений в папке "Входящие" учетной записи. Запустив приложение, вы сможете открыть файл GetStartedWithEWS.log и просмотреть XML-запрос, отправленный на сервер Exchange Server, и возвращенный сервером отклик.</span><span class="sxs-lookup"><span data-stu-id="64355-p114">Add the following code to the  `ShowNumberOfMessagesInInbox` method that was stubbed out after the main method. When you run the application, it will print the number of messages in the account's Inbox and the number of unread messages in the Inbox. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span> 
  
```cs
      /// This is the XML request that is sent to the Exchange server.
      var getFolderSOAPRequest =
"<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
"<soap:Envelope xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\"\n" +
"   xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
"<soap:Header>\n" +
"    <t:RequestServerVersion Version=\"Exchange2007_SP1\" />\n" +
"  </soap:Header>\n" +
"  <soap:Body>\n" +
"    <GetFolder xmlns=\"https://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
"               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\">\n" +
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
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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
                                              ("{https://schemas.microsoft.com/exchange/services/2006/messages}Folders")
                                            select folderElement;
            foreach (var folder in folders)
            {
              Tracing.Write("Folder name:     ");
              var folderName = from folderElement in
                                 folder.Descendants
                                 ("{https://schemas.microsoft.com/exchange/services/2006/types}DisplayName")
                               select folderElement.Value;
              Tracing.WriteLine(folderName.ElementAt(0));
              Tracing.Write("Total messages:  ");
              var totalCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}TotalCount")
                               select folderElement.Value;
              Tracing.WriteLine(totalCount.ElementAt(0));
              Tracing.Write("Unread messages: ");
              var unreadCount = from folderElement in
                                 folder.Descendants
                                   ("{https://schemas.microsoft.com/exchange/services/2006/types}UnreadCount")
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

### <a name="send-an-email-message"></a><span data-ttu-id="64355-160">Отправка электронных сообщений</span><span class="sxs-lookup"><span data-stu-id="64355-160">Send an email message</span></span>

<span data-ttu-id="64355-p115">Отправка электронных сообщений или приглашений на собрания — это еще одна типовая операция приложения EWS. Данный пример позволяет создать и отправить сообщение с помощью введенных ранее учетных данных пользователя. Пример демонстрирует следующие типовые задачи приложений EWS:</span><span class="sxs-lookup"><span data-stu-id="64355-p115">Another common operation for an EWS application is to send email messages or meeting requests. This example creates and sends an email message using the user credentials that were entered earlier. It demonstrates these common EWS application tasks:</span></span>
  
- <span data-ttu-id="64355-164">создание и отправка электронных сообщений;</span><span class="sxs-lookup"><span data-stu-id="64355-164">Creating and sending an email.</span></span>
    
- <span data-ttu-id="64355-165">анализ возвращенного XML-отклика для определения того, было ли сообщение отправлено корректно;</span><span class="sxs-lookup"><span data-stu-id="64355-165">Parsing the returned XML response to determine if the email was correctly sent.</span></span>
    
- <span data-ttu-id="64355-166">обработка типовых исключений и сообщений об ошибке.</span><span class="sxs-lookup"><span data-stu-id="64355-166">Handling common exceptions and error messages.</span></span>
    
<span data-ttu-id="64355-p116">Добавьте указанный ниже код в метод SendTestEmail, заглушенный вслед за основным. Запустив приложение, вы можете открыть файл GetStartedWithEWS.log и просмотреть XML-запрос, отправленный на сервер Exchange Server, и возвращенный сервером отклик.</span><span class="sxs-lookup"><span data-stu-id="64355-p116">Add the following code to the SendTestEmail method that was stubbed out after the main method. After you run the application, you can open the GetStartedWithEWS.log file to see the XML request that was sent to the Exchange server and the response that the server returned.</span></span>
  
```cs
var createItemSOAPRequest =
      "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
      "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\" \n" +
      "               xmlns:m=\"https://schemas.microsoft.com/exchange/services/2006/messages\" \n" +
      "               xmlns:t=\"https://schemas.microsoft.com/exchange/services/2006/types\" \n" +
      "               xmlns:soap=\"https://schemas.xmlsoap.org/soap/envelope/\">\n" +
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
                                               ("{https://schemas.microsoft.com/exchange/services/2006/messages}ResponseCode")
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

## <a name="next-steps"></a><span data-ttu-id="64355-169">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="64355-169">Next steps</span></span>

<span data-ttu-id="64355-p117">Теперь, когда вы написали свое первое приложение EWS, можно переходить к другим способам использования EWS. Вот несколько идей для начала работы:</span><span class="sxs-lookup"><span data-stu-id="64355-p117">Now that you've written your first EWS application, you're ready to discover other ways to use EWS. Here are some ideas to get you started:</span></span>
  
- <span data-ttu-id="64355-p118">Реализуйте в приложении функции [автообнаружения](autodiscover-for-exchange.md), чтобы оно могло соединиться с нужным сервером Exchange Server, используя электронный адрес пользователя. См. также пример в статье [Exchange 2013: получение параметров пользователей с помощью автообнаружения](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e).</span><span class="sxs-lookup"><span data-stu-id="64355-p118">Implement [Autodiscover](autodiscover-for-exchange.md) in your application so that your application will connect to the correct Exchange server based on the user's email address. See also the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/Exchange-2013-Get-user-7e22c86e) sample.</span></span> 
    
- <span data-ttu-id="64355-174">Ознакомьтесь со [справкой по EWS](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) для получения дополнительных сведений об EWS.</span><span class="sxs-lookup"><span data-stu-id="64355-174">Look at the [EWS reference](https://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx) for more information about EWS.</span></span> 
    
- <span data-ttu-id="64355-175">Просмотрите список [операций EWS](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) для получения сведений о доступных операциях.</span><span class="sxs-lookup"><span data-stu-id="64355-175">See the [EWS operations](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx) for information about the operations that are available.</span></span> 
    
- <span data-ttu-id="64355-176">Используйте [редактор EWS](http://ewseditor.codeplex.com/) для просмотра траффика SOAP, отправляемого на сервер и обратно.</span><span class="sxs-lookup"><span data-stu-id="64355-176">Use [EWS Editor](http://ewseditor.codeplex.com/) to see the SOAP traffic sent to and from the server.</span></span> 
    
<span data-ttu-id="64355-177">Если с приложением возникли проблемы, [попробуйте опубликовать вопрос или комментарий на форуме](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (и не забудьте прочитать первую запись).</span><span class="sxs-lookup"><span data-stu-id="64355-177">If you run into any issues with your application, [try posting a question or comment in the forum](https://social.technet.microsoft.com/Forums/exchange/home?forum=exchangesvrdevelopment) (and don't forget to read the first post).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="64355-178">См. также</span><span class="sxs-lookup"><span data-stu-id="64355-178">See also</span></span>

- [<span data-ttu-id="64355-179">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="64355-179">Start using web services in Exchange</span></span>](start-using-web-services-in-exchange.md)   
- [<span data-ttu-id="64355-180">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="64355-180">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [<span data-ttu-id="64355-181">Общие сведения о разработке клиента EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="64355-181">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)   
- [<span data-ttu-id="64355-182">Разработка клиентов веб-служб для Exchange</span><span class="sxs-lookup"><span data-stu-id="64355-182">Develop web service clients for Exchange</span></span>](develop-web-service-clients-for-exchange.md)  
- [<span data-ttu-id="64355-183">Начало работы с клиентскими приложениями, использующими управляемый API EWS</span><span class="sxs-lookup"><span data-stu-id="64355-183">Get started with EWS Managed API client applications</span></span>](get-started-with-ews-managed-api-client-applications.md)
    
