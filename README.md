# Exam-Results-Calculator
A C# Windows Forms app for managing student results. It calculates total scores from class (50%) and exam (50%) marks per subject, ranks students by subject and overall, prevents duplicate entries, and supports PDF/Excel export. Built with SQLite—no external setup needed.

## ✨ Features

- Add and manage students and subjects
- Record class score (50%) and exam score (50%) per subject
- Automatically calculate total scores
- Rank students per subject
- Overall ranking across subjects per class
- Export results to **PDF** and **Excel**
- Prevents duplicate entries using smart validation
- Uses **SQLite** (no external database setup required)

## 📦 Installation

1. Clone or download the repository.
2. Open the solution in **Visual Studio 2022**.
3. Build and run the project.
4. The database file is automatically created in:

## 🧪 Deployment

To create an installable `.exe`:
- Use [Microsoft Visual Studio Installer Projects 2022](https://marketplace.visualstudio.com/items?itemName=VisualStudioClient.MicrosoftVisualStudio2022InstallerProjects) extension
- Package the app into an installer
- The installer includes the SQLite database and required dependencies

## 📁 Data Storage

- Data is stored locally using **SQLite**
- Database file: `exam_results.db`


### 📦 Required NuGet Packages

Make sure the following NuGet packages are installed before building the project:

| Package Name                    | Description                               |
| ------------------------------- | ----------------------------------------- |
| `Microsoft.Data.Sqlite`         | SQLite database provider for .NET         |
| `PdfSharp`                      | For generating PDF files                  |
| `MigraDoc.DocumentObjectModel`  | Used with PdfSharp for formatting content |
| `System.Data.Common`            | Base class library for database access    |
| `System.Drawing.Common`         | For image and graphics handling in .NET   |
| `SQLitePCLRaw.bundle_e_sqlite3` | Enables native SQLite functionality       |

You can install them using the **NuGet Package Manager** in Visual Studio or run the following commands in the **Package Manager Console**:

```bash
Install-Package Microsoft.Data.Sqlite
Install-Package PdfSharp
Install-Package MigraDoc.DocumentObjectModel
Install-Package System.Drawing.Common
Install-Package SQLitePCLRaw.bundle_e_sqlite3
```

## 🤝 Contributions

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

## 📜 License

