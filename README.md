# Project Mu UEFI Implementation for Surface Duo

## Xây dựng

Quick notes for building:

- Dùng Ubuntu bản 20.04 x64
- Tạo ra bảng ACPI với IASL
- Làm theo bản nháp nhanh này

```
# Setup environment
./setup_env.sh

# Activate Workspace
python3 -m venv SurfaceDuo
source SurfaceDuo/bin/activate

# Build UEFI
pip install --upgrade -r pip-requirements.txt
./build_uefi.sh

# Generate ELF image
./build.sh
```

## Acknowledgements

- [EFIDroid Project](http://efidroid.org)
- Andrei Warkentin and his [RaspberryPiPkg](https://github.com/andreiw/RaspberryPiPkg)
- Sarah Purohit
- [Googulator](https://github.com/Googulator/)
- [Ben (Bingxing) Wang](https://github.com/imbushuo/)
- [Renegade Project](https://github.com/edk2-porting/)

## License

All code except drivers in `GPLDriver` directory are licensed under BSD 2-Clause. 
GPL Drivers are licensed under GPLv2 license.
