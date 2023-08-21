(2) Aprire un pacchetto di figurine

prendo n pachetti di figurine
mi avvicino al tavolo
mi siedo sulla sedia
sposto la sedia

# start loop
-finchè ho buste 
    - apro una busta 
        - prendo le carte in mano 
        - le controllo
            - SE figurina = rotta/dannegiata 
                - aggiungi a scarti 
            
            - ALTRIMENTI {
                
                tieni
                
                - SE carta nuova aggiungi a "Album principale" 

                - ALTRIMENTI // carta = doppiona 
                    aggiungi ALBUM scambi

                    - SE carta in album scambi >= 2
                        scambia con amico 

                    - ALTRIMENTI 
                        tieni 

                }

    - riciclo busta    
# end loop


# start loop
- apro una busta 
    - prendo le carte in mano 
    - le controllo
        - SE figurina = rotta/dannegiata 
            - aggiungi a scarti 
        
        - ALTRIMENTI figurina = integra tieni
            - dividi per categoria [comune, noncomune, raro, epico, legy] 
                - SE carta nuova aggiungi a ALBUM principale 

                - ALTRIMENTI carta = doppiona aggiungi ALBUM scambi
                SE carta in album 2 = >= 2 scambia con amico 
                ALTRIMENTI tieni 
- riciclo busta         
# end loop
# start loop
- apro una busta in cerca di drago x 
    - prendo le carte in mano 
    - le controllo
        - SE figurina = drago x smetti di comprare
        
        - ALTRIMENTI figurina = integra tieni
            -aggiungi ad album 
                -SE doppiona aggiungi a "scambi con amici"
            -compra ancora 
-ricicla busta

# end loop