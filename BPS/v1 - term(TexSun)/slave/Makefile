# MPLAB IDE generated this makefile for use with GNU make.
# Project: slave.mcp
# Date: Tue Aug 28 00:12:04 2012

AS = pic30-as.exe
CC = pic30-gcc.exe
LD = pic30-ld.exe
AR = pic30-ar.exe
HX = pic30-bin2hex.exe
RM = rm

slave.hex : slave.cof
	$(HX) "slave.cof"

slave.cof : main.o SPI.o LTC6803.o RS485slave.o ADC.o registers.o slave_misc.o eeprom_rw.o
	$(CC) -mcpu=30F6012A "main.o" "SPI.o" "LTC6803.o" "RS485slave.o" "ADC.o" "registers.o" "slave_misc.o" "eeprom_rw.o" -o"slave.cof" -Wl,--script="C:\Program Files\Microchip\MPLAB C30\support\dsPIC30F\gld\p30F6012A.gld",--defsym=__MPLAB_BUILD=1,--defsym=__MPLAB_DEBUG=1,--defsym=__MPLAB_DEBUGGER_ICD2=1,--defsym=__ICD2RAM=1,-Map="slave.map",--report-mem

main.o : RS485slave.h variables.h c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30Fxxxx.h main.c
	$(CC) -mcpu=30F6012A -x c -c "main.c" -o"main.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

SPI.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h SPI.c
	$(CC) -mcpu=30F6012A -x c -c "SPI.c" -o"SPI.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

LTC6803.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h LTC6803.c
	$(CC) -mcpu=30F6012A -x c -c "LTC6803.c" -o"LTC6803.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

RS485slave.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h RS485slave.c
	$(CC) -mcpu=30F6012A -x c -c "RS485slave.c" -o"RS485slave.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

ADC.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h ../common/ADC.c
	$(CC) -mcpu=30F6012A -x c -c "D:\solar car\texsun\BPS\firmware\v1\common\ADC.c" -o"ADC.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

registers.o : ../common/eeprom_rw.h c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h ../common/registers.c
	$(CC) -mcpu=30F6012A -x c -c "D:\solar car\texsun\BPS\firmware\v1\common\registers.c" -o"registers.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

slave_misc.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/h/p30F6012A.h slave_misc.c
	$(CC) -mcpu=30F6012A -x c -c "slave_misc.c" -o"slave_misc.o" -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 -g -Wall

eeprom_rw.o : c:/program\ files/microchip/mplab\ c30/support/dsPIC30F/inc/p30f6012a.inc ../common/eeprom_rw.s
	$(CC) -mcpu=30F6012A -c -D__DEBUG -D__MPLAB_DEBUGGER_ICD2=1 "D:\solar car\texsun\BPS\firmware\v1\common\eeprom_rw.s" -o"eeprom_rw.o" -Wa,--defsym=__DEBUG=1,--defsym=__MPLAB_DEBUGGER_ICD2=1,-g

clean : 
	$(RM) "main.o" "SPI.o" "LTC6803.o" "RS485slave.o" "ADC.o" "registers.o" "slave_misc.o" "eeprom_rw.o" "slave.cof" "slave.hex"

