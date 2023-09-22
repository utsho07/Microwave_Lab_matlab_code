clc;
clear all;
close all;

Am=input('Enter message signal amplitude: '); %message signal amplitude
Ac=input('Enter carrier signal amplitude: '); %carrier signal amplitude
fm=input('Enter message frequency: '); %message signal frequency
fc=input('Enter carrier frequency: '); %carrier signal frequency
t=input('Enter time period: '); %time period
m=input('Enter modulation index: ');
%%======================================================================================

t1=linspace(0,t,1000);
y1=Am*cos(2*pi*fm*t1); % message signal
y2=Ac*cos(2*pi*fc*t1); % carrier signal
eq=Ac*cos(2*pi*fc*t1)+((m*Ac)/2)*cos(2*pi*fc*t1+2*pi*fm*t1)+((m*Ac)/2)*cos(2*pi*fc*t1-2*pi*fm*t1);%modulated signal
subplot(311);
%%=======================================================================================

plot(t1,y1);
xlabel('Time');
ylabel('Amplitude');
title('Message signal')
subplot(312)
plot(t1,y2);
xlabel('Time');
ylabel('Amplitude');
title('Carrier signal');
subplot(313);
plot(t1,eq);
plot(t1,eq,'r');
xlabel('Time');
ylabel('Amplitude');
title('Modulated signal');
