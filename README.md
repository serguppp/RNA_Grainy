# RNAGrainy
> Uniwersalna platforma do generowania, wizualizacji i porównywania modeli gruboziarnistych (coarse-grained) struktur RNA.

To repozytorium jest publicznym klonem projektu utworzonym na potrzeby prezentacji portfolio.

![Stack](https://img.shields.io/badge/Stack-FastAPI%20%7C%20HTMX%20%7C%20Alpine.js%20%7C%20Tailwind%20%7C%20Gemmi-blue)

## O projekcie
RNAGrainy to specjalistyczne narzędzie webowe dedykowane bioinformatykom, umożliwiające transformację pełnoatomowych struktur RNA do uproszczonych modeli gruboziarnistych (coarse-grained). Projekt rozwiązuje problem braku uniwersalnej platformy integrującej różne modele obliczeniowe stosowane w symulacjach biologicznych.

## Kontekst Naukowy
Modelowanie dynamiki RNA jest kluczowe dla zrozumienia ich funkcji biologicznych. Ze względu na ogromną złożoność obliczeniową struktur pełnoatomowych (45,4 mln znanych sekwencji vs tylko 2 tys. struktur RNA w PDB), bioinformatyka wykorzystuje modele gruboziarniste. RNAGrainy wypełnia lukę w narzędziach pozwalających na szybkie generowanie i porównywanie tych reprezentacji.

## Kluczowe funkcjonalności
- **Import danych:** Obsługa formatów PDB/CIF oraz bezpośrednia integracja z bazą RCSB PDB (poprzez PDB ID). Możliwość wyboru struktur predefiniowanych.
- **Wybór modeli:** Wybór predefiniowanych modeli gruboziarnistych pochodzących z literatury naukowej z możliwością selekcji konkretnych łańcuchów i modeli struktury.
- **Interaktywna wizualizacja:** Porównanie modelu wejściowego i wynikowej reprezentacji gruboziarnistej za pomocą biblioteki Molstar.
- **Kreator własnych modeli:** Moduł pozwalający na definiowanie własnych, niestandardowych reprezentacji gruboziarnistych.
- **Eksport:** Zapis wyników do standardowych formatów PDB/CIF.
- **Dokumentacja:**  Opisy teoretyczne modeli oraz odnośniki do literatury źródłowej.

## Stack Technologiczny
- **Backend:** Python (FastAPI)
- **Frontend:** HTMX & Alpine.js
- **Stylizacja:** Tailwind CSS.
- Gemmi – biblioteka wykorzystywana do precyzyjnej manipulacji i transformacji modeli makrocząsteczek.
  
# Prezentacja aplikacji

<img width="1919" height="1077" alt="main_page" src="https://github.com/user-attachments/assets/1056f8c2-bfa8-416d-b682-a13d3abb7e4b" />

<em>Rys. 1: Interfejs główny aplikacji – responsywny formularz (Tailwind CSS) umożliwiający pobieranie struktur bezpośrednio z bazy RCSB PDB lub przesyłanie własnych plików PDB/CIF.</em>

<img width="1919" height="1079" alt="main_page2" src="https://github.com/user-attachments/assets/b84d1125-5644-4a5b-98e3-fd8a616f6eaa" />

<em>Rys.2: Widok strony głównej z wypełnionym polem wgrania pliku oraz wybranym modelem Custom Model. Na zrzucie ekranu widać przyciski, które pojawiają się po wyborze opcji niestandardowego modelu. </em>

<img width="1919" height="1079" alt="creator" src="https://github.com/user-attachments/assets/2b75fbe7-815c-49d9-aff0-d366a53093e7" />

<em>Rys.3:  Widok kreatora wyświetlany po naciśnięciu przycisku Create Model</em>

<img width="1919" height="1079" alt="creator2" src="https://github.com/user-attachments/assets/9acc9db0-e584-4225-9be3-62293a221e3f" />

<em>Rys.4:  Widok kreatora i pól konfiguracyjnych pseudoatomów </em>

<img width="1917" height="1077" alt="creator3" src="https://github.com/user-attachments/assets/b36458da-4207-4530-9ef2-4c2c95ec8e9e" />

<em>Rys.5: Widok kreatora i pól konfiguracyjnych połączeń między zdefiniowanymi pseudoatomami. </em>

<img width="1919" height="1079" alt="comparison" src="https://github.com/user-attachments/assets/c1f18aea-8d2c-4595-810d-05e0e9ab38e1" />

<em>Rys.6: Widok wyników wyświetlany po zakończeniu procesu uziarniania struktury. </em>

<img width="1919" height="1079" alt="comparison-desc" src="https://github.com/user-attachments/assets/92f45960-6fd0-4198-ad9d-21c31e6c5d84" />

<em>Rys.7:  Widok wyników z rozwiniętą sekcją opisu modelu. </em>

<img width="1910" height="1079" alt="comparison-cit" src="https://github.com/user-attachments/assets/5253c775-170f-41aa-b86a-26e051ff0f02" />

<em>Rys.8: Widok wyników z rozwiniętą sekcją literatury źródłowej, na której oparto opis modelu. </em>

<img width="1918" height="1079" alt="mapping" src="https://github.com/user-attachments/assets/9c7d5739-7616-4f6d-af97-c9f7ba4c5a92" />

<em>Rys.9: Widok wyników z rozwiniętą sekcją mapowania atomów. </em>

<img width="1919" height="1079" alt="molstar" src="https://github.com/user-attachments/assets/a008365b-c76f-425f-bd99-ac2c3b2fe898" />

<em>Rys.10: Widok wizualizatora Mol* i reprezentacji gruboziarnistej cząsteczki 1MNX w modelu SimRNA.</em>

<img width="1901" height="1079" alt="documentation-page" src="https://github.com/user-attachments/assets/892c73d8-1d55-49f8-87f8-99e27a429e83" />

<em>Rys.11: Widok dokumentacji wyświetlany po wejściu na jej stronę. </em>

<img width="1899" height="1079" alt="documentation-feb" src="https://github.com/user-attachments/assets/292547e2-b444-491a-8ba1-6010c49ed404" />

<em>Rys.12: Widok dokumentacji modelu FebRNA z rozwiniętymi regułami mapowania dla puryn i pirymidyn. </em>

