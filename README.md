```cpp
// EmrePekerProfile.java

public class Emrepkeer Profile {

    // Kişisel bilgiler
    private final String firstName = "Emre";
    private final String lastName = "Peker";

    // Bildiği programlama dilleri
    private final String[] knownLanguages = {
        "Java", "C++", "C#", "HTML", "PHP", "JSON"
    };

    // Ana uzmanlık alanı
    private final String primaryLanguage = "Java";

    // Kişisel mottolar ve değerler
    private final String[] passions = {
        "Clean Code", "Problem Solving", "Continuous Learning", "Efficient Algorithms"
    };

    // Projelerde öncelik verdiği özellikler
    private final String[] focusAreas = {
        "Scalability", "Performance", "Maintainability", "Readability"
    };

    public void displayProfile() {
        System.out.println("== Emrepkeer - Developer Profile ==");
        System.out.printf("Name: %s %s%n", firstName, lastName);
        System.out.println("Primary Language: " + primaryLanguage);
        
        System.out.print("Known Languages: ");
        for (String lang : knownLanguages) {
            System.out.print(lang + " ");
        }
        System.out.println("\n");

        System.out.print("Passions: ");
        for (String passion : passions) {
            System.out.print(passion + " | ");
        }
        System.out.println("\n");

        System.out.print("Focus Areas: ");
        for (String focus : focusAreas) {
            System.out.print(focus + " | ");
        }
        System.out.println("\n");

        System.out.println("Contact: emre.peker@example.com");
        System.out.println("GitHub: https://github.com/emrepeker");
        System.out.println("====================================");
    }

    public static void main(String[] args) {
        EmrePekerProfile profile = new Emrepkeer Profile();
        profile.displayProfile();
    }
}
```
