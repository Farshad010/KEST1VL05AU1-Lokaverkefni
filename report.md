# KEST1VL05AU1 - Lokaverkefni

## Dagbók
- **Dagur 1:** Búið til notendareikninga og hópa.
- **Dagur 2:** Stillt réttindi fyrir möppur.
- **Dagur 3:** Stillt heimasvæði og læst reikningum.
- **Dagur 4:** Uppsett Zsh og stillt sudo fyrir Áslaug.

## Leiðbeiningar fyrir Áslaug

### 1. Hvernig á að búa til nýjan notanda:
Til að búa til nýjan notanda með viðeigandi heimasvæði og skel, notaðu eftirfarandi skipun:   `sudo useradd -m -s /bin/bash -c "Fullt Nafn" notendanafn`
Þessi skipun býr til nýjan notanda með heimasvæði og `bash` skel (útfærðu eftir þörfum). Fyrir þig, Áslaug, verður notað Zsh í staðinn fyrir Bash:  
`sudo useradd -m -s /bin/zsh -c "Áslaug Hauksdóttir" aslaug`

### 2. Setja notendur í réttan hóp
Til að bæta notanda í hóp (til dæmis í `forritun ` hóp), skaltu keyra þessa skipun: `sudo usermod -aG forritun notendanafn`

### 3. Láta Erlendur og Erla ekki skrá sig inn
Ef þú vilt læsa aðgangi Erlendar og Erla, getur þú keyrt þessar skipanir:
`sudo usermod -L erlendur`  
`sudo usermod -L erla`  

### 4. Virkja aðgang Erlendar og Erla aftur
`sudo usermod -U erlendur`  
`sudo usermod -U erla`
