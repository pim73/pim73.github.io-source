---
title: "Linode i Organice"
date: 2021-05-27T10:41:21+02:00
categories: ["narzędzia"]
tags: ["emacs"]
---
W nawiązaniu do mojego wpisu z [2021-04-14](https://pim73.github.io/posts/emacs/) dotyczącego dostępu do mojej Org Agendy znalazłem dwa świetne rozwiązania, którymi chcę się podzielić. 

##  Organice
[Organice](https://organice.200ok.ch) to aplikacja webowa, z możliwością zainstalowania jako aplikację PWA (Progressive Web Application)

Należy zalogować się za pomocą konta Dropbox lub Google Drive i udostępnić pliki `org` w odpowiednim folderze. 

**Zalety**:

- można różne pliki dodać do agendy
- Dostęp w telefonie oraz tablecie 
- rozwiązanie całkowicie darmowe 
- dość szybkie oswojenie się z tym rozwiązaniem 

**Wady**:

- niezbyt przejrzysty sposób edytowania plików, ale to chyba w ogóle trudne, gdy korzysta się z klawiatury ekranowej w telefonie
- do wykorzystania raczej doraźnie

##  [Linode](linode.com) lub jakiś inny VPS

W iPadzie zainstalowałem aplikację [Blink](https://blink.sh) i za pomocą `SSH` łączę się z moim Ubuntu na serwerze, a tam korzystam swobodnie z emacsa, orgmode i wszystkich terminalowych aplikacji, do których się przyzwyczaiłem. 

Aby połączyć się z plikami z mojego komputera, wykorzystuję terminalową wersję `Dropboxa`. Instrukcje, w jaki sposób można zainstalować dropbox za pomocą terminala na serwerze można bez trudu znaleźć w sieci. Synchronizacja działa bezbłędnie, więc właściwie nie ma to w tej chwili dla mnie znaczenia, czy edytuje moje pliki `.org` na moim komputerze czy raczej korzystam z linuxa za pośrednictwem `Blink` na iPadzie.

**Zalety**

- korzystam z pełnowartościowego Emacsa i dodatkowo mam dostęp do wielu innych aplikacji dostępnych na terminal linuxa

**Wady**

- głównie koszty. Za `Blink` trzeba zapłacić jednorazowo ok 20 USD oraz za VPS 5 USD miesięcznie
- trudność. Trzeba już mieć choćby niewielkie doświadczenie i wiedzę o linux, serwerach, ssh

## Podsumowanie
Na razie to najdoskonalsze rozwiązanie, jakie znalazłem. Być może istnieją jakieś prostsze lub tańsze, ale na razie wykorzystuję wspomniany w poście sposób.
