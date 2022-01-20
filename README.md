# AM-Modulation
% Hz olarak Taşıyıcı Frekans girişi yapılıyor
Fc = input('Taşıyıcı Frekansı Giriniz: ')
 
% Hz olarak Mesaj Sinyali girişi yapılıyor (Fs > 2Fc)
Fs= input('Mesaj Sinyalini Giriniz: ')
 
% Artan zaman değeri
t = (0 : 1 / Fs : 8);
 
% 't' süreli cosinüs dalgası
x = cos(2*pi*t);
  
% Amplitude Modulation
y = ammod(x, Fc, Fs);
 
plot(y);
title('Amplitude Modulation');
xlabel('Zaman(sn)');
ylabel('Genlik');
