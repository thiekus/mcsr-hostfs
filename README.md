# Midnight Club: Street Racing HostFS Unpacked

My attempt to recreate lost Project AGE for running Midnight Club: Street Racing (NTSC-US `SLUS_200.63` and PAL-EU v1.2 `SLES_500.71` Nov 28th 2000) with unpacked files as pnach patch. To use this:

* Make sure in PCSX2 (v2.x) enable `Tools > Show Advanced Settings`.
* Put `DFD26C76.pnach` (for NTSC-US) or `831078BD.pnach` (for PAL-EU v1.2) patch file into PCSX2 patches directory.
* Copy all CD contents into directory.
* Use ar or `dave.py` to extract *.DAT files into subdirectory (e.g. `FRONTEND.DAT` -> `FRONTEND`). Except for `CARS.DAT` you can use 7zip or winrar to extract. Delete `System.cnf` for extracted file from PAL version if exists.
* For each extracted subdirectory, cut any folders of `CARS`, `COMMON`, `FRONTEND`, `L01` and `M01` into root directory of extracted CD contents. Just overwrite all if asked.
* Delete `CARS.DAT`, `COMMON.DAT`, `FRONTEND.DAT`, `L01.DAT` and `M01.DAT`. Also created folders of each archives subdirectory before.
* Rename `SLUS_200.63` (NTSC-US) or `SLES_500.71` (PAL v1.2) into `mc.elf`.
* Add that extracted CD directory into PCSX2 game list. Right select to newly added `mc` and click Properties.
* On summary, make sure Disc Path is points to your original ISO/Image (to able game to first boot).
* On Emulation, make sure you "Enable Host Filesystem".
* On Patches, Enable "HostFS Unpacked" patch.
* Just click `mc` game entry to play MCSR unpacked!
