# Library-management-system-Libraray Management System:
class User {
    String name;
    String userId;

    public User(String name, String userId) {
        this.name = name;
        this.userId = userId;
    }
}

class Librarian extends User {
    public Librarian(String name, String userId) {
        super(name, userId);
    }

    public void addBook(Book book) {
        System.out.println("Book added: " + book.title);
    }

    public void removeBook(Book book) {
        System.out.println("Book removed: " + book.title);
    }
}

class Book {
    String title;
    String author;
    String isbn;
    boolean isAvailable;

    public Book(String title, String author, String isbn, boolean isAvailable) {
        this.title = title;
        this.author = author;
        this.isbn = isbn;
        this.isAvailable = isAvailable;
    }
}

class Account {
    String username;
    String password;
    boolean isActive;

    public Account(String username, String password, boolean isActive) {
        this.username = username;
        this.password = password;
        this.isActive = isActive;
    }
}
