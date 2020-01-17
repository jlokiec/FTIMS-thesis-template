## Ogólnie  
Szablon LaTeX wykorzystany do napisania pracy inżynierskiej na Politechnice Łódzkiej, kierunek informatyka, wydział FTIMS.  
Zapewnia:
- odpowiednie formatowanie tekstu,
- automatyczne generowanie spisu rysunków, listingów i tabel,
- zarządzanie bibliografią.  

Przykładowy wygenerowany plik PDF: [example.pdf](example.pdf).  

## Wstawianie rysunków  
Pliki rysunków należy umieścić w folderze `img`. Przykład wstawienia rysunku w pracy znajduje się w pliku [main.tex](main.tex).  

## Bibliografia  
Wpisy z literaturą należy umieścić w pliku [bibliography.bib](bibliography.bib). Odniesienie do pozycji z bibliografii w kodzie LaTeX odbywa się poprzez instrukcję `\cite{nazwa_pozycji}`.  

## Narzędzia  
Do pisania pracy można wykorzystać zarówno aplikacje webowe jak i desktopowe.  
Darmowym webowym środowiskiem LaTeX jest np. [Overleaf](https://www.overleaf.com/).  
Jeżeli chcesz korzystać z aplikacji desktopowych, zapoznaj się z [listą środowisk LaTeX](https://tex.stackexchange.com/questions/339/latex-editors-ides).

## Konfiguracja LaTeX  
Jeżeli chcesz kompilować dokumenty LaTeX-a lokalnie, niezbędne będzie zainstalowanie odpowiednich pakietów. Proces instalacji dla Ubuntu 19.10 (jeżeli używasz innej wersji bądź dystrybucji, nazwy pakietów mogą się różnić):
- odśwież repozytoria i zaktualizuj zainstalowane pakiety poleceniem:  
`# apt update && apt upgrade`
- zainstaluj nowe pakiety:  
`# apt install biber texlive-bibtex-extra texlive-lang-polish texlive-latex-extra texlive-fonts-recommended texlive-latex-base`  

Do wygenerowania pliku PDF należy wykonać polecenia:
```
$ pdflatex main.tex
$ biber main
$ pdflatex main.tex
```  
Po wykonaniu powyższych poleceń kompilator wygeneruje wynikowy plik main.pdf.  

#### Wykorzystane zasoby  
Użyte zdjęcie: https://www.pexels.com/photo/blur-close-up-code-computer-546819/
