# Csip Csip
## Csapatnév: Bitang mélyen tanulók
## Csapattagok
- Benedek Zoltán, VZ9AS0
- Biró Márton, Z7A244
- Vizi Kristóf Levente, GN2VV4
## Projekt ismertetése
A projekt célja neurális háló tanítása madarak fajtájának felismerésére a hanguk alapján. Az adathalmaz madarak hanfelvételeiből áll .ogg fileformátumban és 2 darab .csv file-ok melyek a hangfelvételekhez és a madárfajokhoz tartalmaznak információkat.

**Kaggle link a feladathoz:** https://www.kaggle.com/competitions/birdclef-2024

### Beszámoló pdf neve
**Beszámoló.pdf**
Megajánlott jegyért

## Első milestone-ra beadott ipyn file neve
**BirdCLEF.ipyn**

*Ebben a Google Colab munkafüzetben zajlik az adatok feldolgozása és tanítás adatainak vizualizálása.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/BirdCLEF.ipynb)


## Végleges projekt file-jainak funkciói

**Upload_training_data_to_drive.ipynb**

*Ebben a munkafüzetben egy olyan kódsorozat szerepel mely a Kaggle oldaláról letölti a megfelelő zipfile-t, majd ezt egy Google Drive mappába feltöltve kicsomagolja hogy a későbbi használatra mindig elérhetőek legyenek a file-ok. Ezen kívül egy kisebb tanítóhalmazt is létrehoz.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Upload_training_data_to_drive.ipynb)



**Data_visualization.ipynb**

*Ebben a munkafüzetben szerepel a kapott adatok vizualizációja.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Data_visualization.ipynb)



**Saving_spectrograms_to_disk_final_faster.ipynb**

*Az ebben szereplő kódrész az audiófájlok első 5 másodperces részét spektrogrammá alakítja, majdfeltölti a train_spectrograms Google Drive mappába.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Saving_spectrograms_to_disk_final_faster.ipynb)



**Filter_spectrograms_with_Google_classifier.ipynb**

*Ez a munkafüzet átfuttatja a hangfájlokat a Google Bird Vocalization Classifier-en, és az eredménytől függően törli, vagy áthelyezi azok spektrogramját.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Filter_spectrograms_with_Google_classifier.ipynb)



**Audio_augmentation.ipynb**

*Ebben a munkafüzetben vannak az adatdúsításért felelős kódrészek.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Audio_augmentation.ipynb)



**Cross_valid_Train_Uj_Uj.ipynb**

*A spektrogramok betöltésére, duplikált spektrogramok kiszűrésére, és a neurális háló tanítására, kiértékelésére szolgáló munkafüzet.*

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Bitang-Melyen-Tanulok/Csip_Csip/blob/main/Cross_valid_Train_Uj_Uj.ipynb)
