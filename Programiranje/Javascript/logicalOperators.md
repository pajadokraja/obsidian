#javascript 

[[operator]] koji rade logiku na [[boolean]]
&& - i
|| - ili
! - ne
?? - [[null]]ish concealning

&& prolazi kroz sve operande dok ne nadje prvi koji je netacan, i onda vraca njegovu originalnu vrednost. Ako su svi tacni onda vraca poslednji.

|| prolazi kroz sve operande dok ne nadje prvi koji je tacan, i onda vraca njegovu originalnu vrednost. Ako su svi netacni onda vraca poslednji.

! pretvori vrednost operanda u boolean i onda vrati njegov inverz.

?? vrati prvu vrednost ako je prva vrednost definisana, drugu ako prva vrednost nije definisana