# Digital Diary

## 🧩 Project Description and Features
A *Digital Diary* that allows users to maintain personal diary entries. This offers two modes: a **normal diary** and a **secure diary**. Each entries are stored in text files, with timestamps automatically added to each entry.

1. Two Diary Modes
	- 📓 Normal Diary
	- 🗝 Secured Diary

2. Core Functionality
	- ✍️ Write Entry: Add new timestamped entries to the diary
	- 📖 View Entries: Display all saved diary entries
	- 🔍 Search by Date: Find entries from a specific date format (YYYY-MM-DD)
	- 🖊️ Edit Entry: Modify existing diary entries
	- ❌ Delete Entry: Remove entries from the diary

## 🧠 How OOP Principles are Used
This diary application leverages the core principles of Object-Oriented Programming (OOP): Encapsulation, Abstraction, Inheritance, and Polymorphism— to build a clean, extensible, and maintainable codebase.

1. 🔐**Encapsulation**
	- is achieved by grouping related data and methods inside classes like Diary and SecureDiary. Internal file operations (ReadAllLinesToList, WriteLinesToFile) are hidden from external acces and exposed through public methods such as WriteEntry, EditEntry, and DeleteEntry.
	- the password in SecureDiary is stored in a private field (_password) and accessed internallu, ensuring it's not exposed to outside classes.
2. 🎯 **Abstraction**
	- is demonstrated through the use of the IDiary interface
	- IDiary defines essential diary operations like WriteEntry, GetAllEntriesAsList, SearchByDate, etc., without ecposing implementation details.
	- consumers of the diary interact with the diary through the IDiary interface, allowing flexibility in swapping implementations.
3. 🧬 **Inheritance**
	- is used by extending the base Diary class into a more specialized SecureDiary.
	- SecureDiary inherits standard diary functionality and overrides only the necessary parts to add password protection (e.g., reading/writing entries).
	- this prevents code duplication and promotes reuse.
4. 🔁 **Polymorphism**
	- is utilized through method overriding in SecureDiary (ReadAllLinesToList, WriteLinesToFile) to change behavior while preserving the interface.
	- the ability to reference both Diary and SecureDiary using the IDiary interface, enabling flexible nd interchangeable diary usage.

## 🧑‍🏫 Instruction on Running the App
Follow these steps to run the **DigitalDiary** application smoothly on your local machine:

### 🧰 Prerequisites

Before you start, make sure you have:

- ✅ [.NET SDK (6.0 or later)](https://dotnet.microsoft.com/download)
- ✅ A code editor (we recommend [Visual Studio](https://visualstudio.microsoft.com/) or [VS Code](https://code.visualstudio.com/))
- ✅ Git installed

### 🛠️ Set-up Steps

1. **Clone the Repository**

   ```bash
   git clone https://github.com/your-username/DigitalDiary.git
   cd DigitalDiary

2. **Open the Project**
   #### Option 1: Using Visual Studio
	Open the .sln file:

	```bash
 	File > Open > Project/Solution > DigitalDiary.sln
 	```
   #### Option 2: Using CLI or VS Code
   	```bash
   	code .
	```
3. **Run the App**
   #### Use the .NET CLI:
   	```bash
 	dotnet run
 	```
    Or press F5 in Visual Studio to run the app with debugging.

### ✅ How to Use
1. 📝 Choose Diary Type
	- Press 1 for Normal Diary
	- Press 2 for Secured Diary
	- Press 3 to Close Application
2. 🏠 Main Menu
	- Press 1 to Write a New Entry
	- Press 2 to View All Entries
	- Press 3 to Search Entries by Date
	- Press 4 to Edit an Entry
	- Press 5 to Delete an Entry
	- Press 6 to Exit

Just follow the on-screen prompt to use the app.

## 📂 File Structure
![File Structure](sample_output/file-structure.png)

## 🖥 Sample Output
*Start*

![Start](sample_output/start.png)

*Main Menu*

![Main Menu](sample_output/main-menu.png)

*Write*

![Write](sample_output/write.png)

*Search*

![Search](sample_output/search.png)

*Edit*

![Edit](sample_output/edit.png)

*Delete*

![Delete](sample_output/delete.png)

## 🧑‍💻 Team Members
| Name  | E-mail             |
|------------|-------------------------|
| Africa, Kiarra Francesca Gabrielle S. | 23-01292@g.bastate-u.edu.ph |
| Aguzar, Joel Lazernie A. | 23-00562@g.batstate-u.edu.ph |
| Garcia, Kriztel C.| 23-03726@g.batstate-u.edu.ph |
| Lacerna, James Louie | 23-05991@g.batstate-u.edu.ph |

## 🤝 Acknowledgement

We, the members of **GROUP 8**, would like to sincerely thank **Ms. Fatima Marie P. Agdon**, our Advanced Object-Oriented Programming instructor, for her guidance, support, and encouragement throughout this project. Her insights and clear explanations helped us greatly in applying advanced programming concepts effectively.

