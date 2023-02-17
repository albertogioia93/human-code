Aprire un pacchetto di figurine

Ce l’ho, mi manca!

Che emozione, ogni volta che apro un pacchetto nuovo... chissà se troverò quella figurina così rara!
Dopo averle sfilate dal pacchetto, me le passo tra le mani controllando nell’album: attacco subito quelle nuove, mentre le doppie le metto in un mazzetto a parte. Ormai ne sto accumulando diverse, spero di riuscire a combinare diversi scambi sabato con i miei amici!


INIZIO {
    apro il cassetto
    CICLO SE ho un nuovo pacchetto? true {
        lo prendo
        apro il pacchetto
        estraggo le carte dal pacchetto
        butto via il pacchetto appena aperto
        prendo l'album
        apro l'album
        CICLO controllo le carte una ad una (SE ci sono ancora carte) true{
            SE trovo rara? true {
                sono contento
            }
            ALTRIMENTI? false {
                sono triste
            }
            SE è doppioni true{
                aggiungi la carta nella lista delle carte doppioni
            }
            ALTRIMENTI false{
                metto la carta nell'album
            }
        }
        ALTRIMENTI false - carte finite{
            torna all'inizio del ciclo
        }
    }
    ALTRIMENTI{
        SE è sabato true{
            chiamo i miei amici
            SE ci sono gli amici e hanno carte da scambiare true{
                organizzo un appuntamento con loro
                prendo la lista dei doppioni
                esco da casa
                li raggiungo
                CICLO confrontiamo le nostre liste dei doppioni ad una ad una fino a quando non finiscono le carte true{
                    SE ho già la carta nell'album e nella lista doppioni true{
                        non faccio niente
                    }
                    ALTRIMENTI false{
                        faccio lo scambio
                    }
                }
            }
            ALTRIMENTI false{
                non faccio niente
            }
        }
        ALTRIMENTI false{
            aspetto sabato
        }
    }
} FINE