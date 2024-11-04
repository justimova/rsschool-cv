# Julia Ustimova
## Junior software developer (C\#)
\+48519434592  
Discord: jayzjay.   
Email: [juli.ustimova@gmail.com](mailto:juli.ustimova@gmail.com)   
GitHub: [https://github.com/justimova](https://github.com/justimova)

## Summary

A graduate of the National Technical University of Ukraine "Kyiv Polytechnic Institute" with a degree in Computer Science. I have fundamental knowledge in software development, algorithms and data structures, object-oriented programming, and working with databases.

For my thesis project, I developed a "Virtual English Tutor Using Artificial Intelligence," utilizing advanced AI technologies to create an interactive educational application.

I’m actively studying new technologies and striving to develop my skills in the fields of artificial intelligence and web programming. I’m seeking opportunities to deepen my knowledge and gain practical experience in application development using C\#, JavaScript, HTML+CSS, and databases.

## Skills

* C\#, JavaScript  
* Entity Framework, LINQ  
* Knowledge of database concepts and knowledge of SQL, design database structure  
* MS SQL Server  
* HTML, CSS

## Code Examples

```
    public void CreateTextForReading(string langLevel, string? authorName, out string title,
			out IList<(string Text, string TranslatedText)> paragraphs) {
		Conversation chat = CreateChatConversation(responseFormat: _jsonResponseFormat);
		chat.AppendSystemMessage(string.Format(_aiSettings.CreateReadingTextSystemMessage,
			_aiSettings.NumberOfWordsForReadingText, langLevel));
		chat.AppendUserInput(string.Format(_aiSettings.CreateReadingTextUserMessage, authorName));
		string response = chat.GetResponseFromChatbotAsync().GetAwaiter().GetResult();
		TextForReading? textForReading = JsonSerializer.Deserialize<TextForReading>(response)
			?? throw new Exception("Something wrong");
		title = textForReading.Title;
		paragraphs = textForReading.Text.Zip(textForReading.TranslatedText,
			(text, translatedText) => (Text: text, TranslatedText: translatedText)).ToList();
    }
```

## Work Experience

### Virtual English Tutor Using Artificial Intelligence

[https://github.com/justimova/EnglishTutorAI](https://github.com/justimova/EnglishTutorAI) 

A web application for learning English without tutors or teachers, using advanced artificial intelligence technologies, providing a personalized approach, high-quality learning, and accessibility to a wide audience.

The web application offers effective and convenient English language learning through interactive sections for reading, writing, grammar study, and working with a dictionary.

Technologies, used within the project: 

* C\#  
* ASP.NET Core  
* TypeScript  
* Entity Framework  
* Web API  
* MS Sql Server  
* Html, CSS, Bootsrtap  
* Angular  
* ChatGPT API

### Service for obtaining the Bitcoin exchange rate

[https://github.com/justimova/genesisTask](https://github.com/justimova/genesisTask) 

A service that provides the latest Bitcoin exchange rate. Additionally, you can subscribe to receive updates on the Bitcoin exchange rate directly to your email.

Technologies, used within the project: 

* JavaScript  
* NodeJS

### Console Application "Organizer"

[https://replit.com/@ustimovajulia/Kriachok-KR-Organizer](https://replit.com/@ustimovajulia/Kriachok-KR-Organizer) 

A console application that enhances the user's work or learning efficiency by organizing tasks in a so-called ToDo list and managing reminders.

The organizer provides the ability to manage reminders and the task list (ToDo). It includes functionality for saving the database to a file on disk, as well as loading it from the disk. When loading from the disk, if there are reminders for the current day, they will be displayed to the user. Additionally, there are service functions for working with the calendar, including displaying the month and the day of the week for a specified date.

Technologies, used within the project: 

* С++

## Education

2020 — 2024

**Bachelor's degree \- National Technical University of Ukraine "Kyiv Polytechnic Institute"**

Department: Information Technologies

Field of study: Computer Science

## English Language
**B2** \- Upper-Intermediate

