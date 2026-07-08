# Кейсы для открытого урока с использованием OpenCV

<div align="center">

[![License](https://img.shields.io/github/license/S0LYER/open-lesson-cases?color=orange&style=flat-square)](LICENSE)
<br>
[![C++](https://img.shields.io/badge/C++-20_|_23-00599C?style=flat-square&logo=cplusplus&logoColor=white)](https://isocpp.org)
[![LLVM](https://img.shields.io/badge/LLVM-18_|_19-262D3A?style=flat-square&logo=llvm&logoColor=white)](https://llvm.org)
[![Clang](https://img.shields.io/badge/Clang-18_|_19-262D3A?style=flat-square&logo=clang&logoColor=white)](https://clang.llvm.org)
<br>
[![Qt6](https://img.shields.io/badge/Qt-6.7_|_6.8-41CD52?style=flat-square&logo=qt&logoColor=white)](https://qt.io)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.10_|_4.11-5C3EE8?style=flat-square&logo=opencv&logoColor=white)](https://opencv.org)
<br>
[![CMake](https://img.shields.io/badge/CMake-3.28_|_3.30-064F8C?style=flat-square&logo=cmake&logoColor=white)](https://cmake.org)
[![Ninja](https://img.shields.io/badge/Ninja-1.12-00A9E0?style=flat-square&logo=ninja&logoColor=white)](https://ninja-build.org)

</div>

Данные кейсы предназначены для открытого урока в вузе. Разработка осуществлялась на Arch linux с использованием Qt6. Библиотека OpenCV собиралась из исходников

---

### Развертка на устройстве: 

```
git clone https://github.com/S0LYER/open-lesson-cases
cd open-lesson-cases
ls
```

---

> [!NOTE]
> Перед компиляцией программы следует перекинуть файлы .qml из папки All_QML в папки qml внутри нужных кейсов

---

### Требуются зависимости:
1. OpenCV (bin/merged)
2. Qt6
3. CMake
4. Ninja
5. LLVM
6. dotnet-sdk
7. GCC

> [!IMPORTANT]
> Я не помню весь список зависимостей, так что в случае ошибок при компиляции/запуске докачайте их лично

---

## Структура проектов

```
case/
├── src/
│   ├── main.cpp
│   ├── videoitem.h
│   ├── videobackend.h
│   ├── videobackend.cpp
├── qml/
│   ├── Main.qml
│   ├── CustomButton.qml
│   ├── PlaybackButton.qml
│   └── WavySlider.qml
└── CMakeLists.txt
```

---

### Сборка на unix-based системах

```
cmake -B build -G Ninja
cmake --build build
```

Запуск:
```
./build/НАЗВАНИЕ_БИНАРНИКА_В КЕЙСЕ  <<=========== Название бинарника будет подсвечено зеленым в списке пакетов после команды "ls build"
```

---
