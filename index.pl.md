---
tytuł: Dokumentacja KOOMPI OS
opis: Dowiedz się, jak korzystać z KOOMPI OS i wszystkich jego narzędzi oraz ustawień.
---

# KOOMPI OS

Doświadcz czystego GNOME na Ubuntu ze szczyptą charakteru.

## FAQ

Odpowiedzi na najczęściej zadawane pytania (chociaż projekt wciąż jest bardzo młody).
- **Dlaczego nowa dystrybucja?**\
  KOOMPI OS powstało z potrzeby stworzenia dystrybucji Linuksa opartej na Ubuntu, 
  która dostarczałaby czyste GNOME bez żadnych zmian w końcowym doświadczeniu 
  użytkownika (user experience). Później jego zakres został rozszerzony, aby 
  poeksperymentować z niektórymi narzędziami i technologiami, takimi jak Almost 
  (niezmienność na żądanie) i pix (podsystem oparty na Distroboxie).
- **Czy wykorzystuje ona OSTree?**\
  Nie. KOOMPI OS osiąga niezmienność poprzez [`almost`](https://github.com/koompi-os/almost). 
  Napisaliśmy to narzędzie z myślą o niezmienności na żądanie opartej na atrybucie 
  "immutability" plików. To podejście działa na każdym schemacie partycji/systemie plików. 
  Wsparcie dla OSTree może zostać dodane jeszcze w przyszłości.
- **Czy rozwijana jest na bazie modelu "rolling release"?**\
  Nie. KOOMPI OS posiada tradycyjny model wydawania aktualizacji i podąża za 
  modelem aktualizacji używanym w Ubuntu.

## Sekcje

- **[Niezmienność (`almost`)](/docs/almost)**\
Almost to narzędzie dla niezmienności na życzenie oparte na atrybucie "immutability" plików. 

- **[Menedżer pakietów (`pix`)](/docs/pix)**\
pix jest menedżerem pakietów, który pozwala na instalację i zarządzanie pakietami 
w zarządzanym kontenerze, bez wpływu na system hosta. Czasami możliwe jest użycie 
`pix` do instalacji pakietów również na systemie hosta.
