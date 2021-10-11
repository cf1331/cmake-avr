## cmake-avr - a cmake toolchain for AVR projects

On this branch the examples have been removed to keep things cleaner when using it as a submodule in other projects.

### Add as submodule

```bash
git submodule add -b no-examples https://github.com/cf1331/cmake-avr.git thirdparty/cmake-avr
```

### Usage

Make sure the AVR toolchain is available in `PATH`.

#### Configure

```bash
mkdir build/
cd build/
cmake -G "Unix Makefiles" -DCMAKE_TOOLCHAIN_FILE=../thirdparty/cmake-avr/generic-gcc-avr.cmake ../
```

#### Build

After configuring, run this in `build/`.

```bash
make
```

#### Upload

The upload command depends on the target name and MCU. Run this in `build/` to find it:

```bash
make help
```


For examples, see [master](https://github.com/cf1331/cmake-avr/tree/master).
