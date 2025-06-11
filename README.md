# Flutter-Book-CRUD-App

Task Objective
A Flutter app that performs CRUD operations on books using:

Clean Architecture (3-layered)

BLoC for state management

Dio for API networking

🔗 API Used:
http://readbuddy-server.onrender.com/api/books


🧱 Architecture
lib/
├── core/                       # (for shared things if needed)
├── features/
│   └── books/
│       ├── data/
│       │   ├── data_sources/   # BookRemoteDataSource with Dio
│       │   ├── models/         # BookModel
│       │   └── repositories/   # BookRepositoryImpl
│       ├── domain/
│       │   ├── entities/       # Book entity
│       │   └── repositories/   # abstract BookRepository
│       └── presentation/
│           ├── bloc/           # book_bloc, book_event, book_state
│           ├── pages/          # UI pages (List, Add, Edit)
│           └── widgets/        # UI widgets (BookItem)
├── main.dart



📦 Packages Used
Package	Usage
flutter_bloc	State management
dio	HTTP API requests
equatable	Simplify BLoC state comparison
flutter_form_builder or forms	Input validation (used native Form)



✨ Features
✅ List all books

➕ Add a new book

✏️ Edit book details

❌ Delete a book

🧱 Clean Architecture & BLoC

🚀 Fully functional API integration
