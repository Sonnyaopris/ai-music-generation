Compoziție Automată de Muzică folosind LSTM, CNN și RNN
Acest repository conține două module principale:

Generare muzică MIDI folosind rețele LSTM.

Generare muzică audio pe baza coeficienților MFCC cu RNN.

Structura Repository-ului
-folder-
├── mfcc_fma_proiect_psv.ipynb        # Generare muzică audio pe baza de coeficienți MFCC
├── midi_AI_generare_muzica.ipynb     # Generare muzică simbolică (MIDI) cu LSTM
└── README.md                         # Acest fișier

Cerințe:
-Python 3.8+

-Google Colab / Jupyter Notebook

-Biblioteci Python: pip install tensorflow numpy pandas music21 pretty_midi librosa matplotlib scikit-learn pyfluidsynth
sudo apt-get install fluidsynth 


- Utilizare-

 midi_AI_generare_muzica.ipynb — Generare pe bază de MIDI
Descriere:
Antrenează un model LSTM pe secvențe de note extrase din fișiere MIDI și generează noi compoziții în funcție de genul selectat.

Pași:

1.Fișierele MIDI au fost organizate manual pe genuri în directorul /data/midi/.

2.Rulează notebook-ul pas cu pas:

      Preprocesare MIDI

      Antrenare model LSTM

      Generare de secvențe noi

3.Output:

    Fișier .mid generat automat

    Conversie în .wav folosind FluidSynth

4.Vizualizare:

   Spectograma fragmentului generat


mfcc_fma_proiect_psv.ipynb — Generare pe bază de MFCC (Audio)

Descriere:
Antrenează o rețea RNN simplă pentru generare audio folosind coeficienți MFCC extrași din fragmente muzicale.

Pași:

1. Baza de date FMA Small a fost folosită. Aceasta poate fi descărcată de la:
https://github.com/mdeff/fma

2.Rulează notebook-ul:

     Extracție MFCC

     Antrenare model LSTM

     Generare de secvențe MFCC noi

3.Output:

     Reconstrucție fișier audio .wav din MFCC generați

4.Vizualizare:

     Spectograma audio generată


Surse Baze de Date
FMA Small Dataset: https://github.com/mdeff/fma

Baza MIDI: organizată manual, fișiere selectate din resurse publice, organizate pe genuri muzicale.

Autor
Opriș Sonnya-Mariana
Universitatea Tehnică din Cluj-Napoca
Facultatea de Electronică, Telecomunicații și Tehnologia Informației
