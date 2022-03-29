# iPXE iso efi-mbr Secureboot Support

credit:

https://github.com/ipxe/ipxe

	1- Türkçe Açıklama

iPXE son sürüm secureboot uyumlu ISO dosyası

Desteklediği platformalar:
- UEFI x86 (secureboot uyumlu)
- UEFI x64 (secureboot uyumlu)
- BIOS-MBR

Bu iso dosyası hem MBR hem de UEFI modunda çalışmaktadır. 

UEFI modunda güvenli önyükleme açık iken de çalışır ancak öncelikle SecureBoot.cer dosyasını BIOS'a tanıtmalısınız.

SecureBoot.cer dosyasının BIOS'a tanıtılması işleminden sonra artık o makinada tekrardan bu işlemi yapmanıza gerek yoktur.

SecureBoot.cer dosyası iso dosyası içinde görünmez. Bu dosya, efi boot sektör dosyası içinde gömülüdür.

Önyükleme esnasında bu dosya görünür olacaktır.

ISO dosyasını Grub2FM, Ventoy, AIO Boot tarzı multiboot yöneticileriyle ön yükleyebilirsiniz.

	2- English Explanation
  
iPXE latest version secureboot support ISO file

Supported platforms:
- UEFI x86 (secureboot support)
- UEFI x64 (secureboot support)
- BIOS-MBR

This iso file works in both MBR and UEFI mode.

It also works in UEFI mode with secure boot turned on, but you must first introduce the SecureBoot.cer file to the BIOS.

After the SecureBoot.cer file is introduced to the BIOS, you do not need to do this again on that machine.

The SecureBoot.cer file does not appear in the iso file. This file is embedded in the efi boot sector file.

This file will be visible during boot.

You can boot the ISO file with Grub2FM, Ventoy, AIO Boot etc. multiboot managers.
