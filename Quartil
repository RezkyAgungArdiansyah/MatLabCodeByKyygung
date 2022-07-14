%Statisctics Find Quartil of Group Data
clc;
clear ;
close all;
DataKelompok = [112 121 130 139 148 157 166;120 129 138 147 156 165  174]';
nilaitengah = mean(DataKelompok,2);
frekuensi = [4 5 8 12 5 4 2]';
fx = nilaitengah.*frekuensi;
Datahasil = [DataKelompok,nilaitengah,frekuensi,fx]
n = sum(frekuensi);
lebardata = DataKelompok(1,2) - DataKelompok (1,1)+1
for i = 1:3
    checker = i*n/4; %misal n = 40 maka checker (1) = 10
  Jkumulatif = 0; j = 1;
  while (Jkumulatif<checker)
     Jkumulatif = Jkumulatif + frekuensi(j);
     j = j+1;
  end
j = j-1;
disp("Kuartil ke - "+i +"terletak pada data ke - "+ j);
Jkumulatif = Jkumulatif - frekuensi(j);
Q (i) = DataKelompok (j,1) + lebardata*(checker - Jkumulatif)/frekuensi(j);
end
Q
