# TPO-charset
TPO - Technologie programowania rozproszonego

# TASK 1

Katalog {user.home}/TPO1dir zawiera pliki tekstowe umieszczone w różnych podkatalogach. Kodowanie plików to Cp1250. Przeglądając rekursywnie drzewo katalogowe, zaczynające się od {user.home}/TPO1dir, wczytywać te pliki i dopisywać ich zawartości do pliku o nazwie TPO1res.txt, znadującym się w katalogu projektu. Kodowanie pliku TPO1res.txt winno być UTF-8.

Poniższy gotowy fragment winien wykonać całą robotę:

```java
public class Main {
    public static void main(String[] args) {
      String dirName = System.getProperty("user.home")+"/TPO1dir";
      String resultFileName = "TPO1res.txt";
      Futil.processDir(dirName, resultFileName);
    }
  }
```

Uwagi!
* pliku Main.java nie wolno w żaden sposób modyfikować,
* trzeba dostarczyć definicji klasy Futil,
* oczywiście, nazwa katalogu i pliku oraz ich położenie są obowiązkowe,
* należy zastosować FileVisitor do przeglądania katalogu oraz kanały plikowe (klasa FileChannel) do odczytu/zapisu plików (bez tego rozwiązanie nie uzyska punktów).
