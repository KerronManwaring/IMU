Igaks juhuks v�ike readme

Tegu on kalman filtri implementatsiooniga. Antud juhul kasutatakse
testkoodis kiirendusanduri ja g�roskoobi v�ljundandmeid ning arvutatakse
nende p�hjal filtrit rakendava seadme asend.

Testkoodi sisendiks on varasemalt �ra salvestatud kalman filtrit
rakendava seadme v�ljundandmed txt faili kujul. V�ljundandmetes
on 3 andmev�lja: Kiirendusanduri andmed, g�roskoobi andmed ja
nende p�hjal jooksutatud kalman filtri tulemus ajasammude l�ikes.

Testkood "kalmanTest.c" v�ljastab need 3 andmev�lja + assembleris
implementeeritud kalman filtri p�hifunktsiooni tulemused. Koodi
eduka t�� tunnus oleks see, et arvutatud tulemused ja varasemalt
m��detud tulemused langevad kokku. Sisendandmete genereerimisel
esineb m�ningaseid �mardusvigasid ning seel�bi v�ivad tulemused
erineda +/- 0.005 v�rra. Samuti ei salvestanud ma �ra algandmete
genereerimisel filtri l�hteasendi ning seet�ttu l�heb testkoodis
filtri stabiliseerimiseks "veidi aega".

Programmi k�ivitamine:

	k�surealt: make all
	k�surealt: kalmanTest.exe ".\Sample Data\sampleData.txt"

T�estus, et programm tegi midagi: pilt "pictures" kaustas.
K�iksugu muu jutt tuleb ette programmi k�ivitades. Osa teksti
ka kalmanTest.c preambulas

Kirjutasin enamasti inglise keeles kuna mul on tavaks panna
k�iksugu v�hegi huvitav ja kellelegi kasulik blogisse �les.
