# IntelHD620FixKREN
지원 중단된 Intel HD 내장 그래픽 620 에서 발생하는 그래픽 화질이 1920x1080이 아닌 1280x1024로 나오는 문제를 해결하는 config.plist 정보를 모두 담은 GitHub 저장소.
A GitHub repository that contains informations of Clover Bootloader's config.plist that fixes the squashed display issue on Intel HD Integrated Graphics 620


# 지원하는 내장 그래픽 Supported iGPU
Intel HD Integraed Graphics 620 인텔 HD 내장 그래픽  620

# 편집할 정보들
*참고로, 이 작업을 원할하게 수행할려면 Clover Configurator의 언어를 영어 (English)로 수정하여야 합니다. NOTE: To proceed this task correctly, please change your Clover Configurator Language to English.

Boot Graphics > Default Background Color: 80000000 (0x80000000)| EFILoginHiDPI: 0 | flagstate: 0 | UIScale: 1

Devices > Fake ID > IntelGFX: 123456789 (0x123456789) | Properties [HEX] > SetIntelBacklight, SetIntelMaxBackligt, UseIntelHDMI: ON 킴

GUI > Screen Resolution: 1920x1080 | PlayAsync, KbdPrevLang, Custom Icons: ON 킴

Graphics > DualLink : 1 | Load VBios, Patch VBios, Inject Intel: ON 킴

Install Drivers > CsmVideoDxe : ON | 클릭 Click Download

저장 Save, Reboot 재시동

끝! Done!

(This document is in Korean and English. 이 문서는 영어와 한국어로 작성되었습니다.
