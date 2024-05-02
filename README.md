# Blink LED on Pico W

Make sure you have the Pico SDK installed and put it into your PATH as `PICO_SDK_PATH`.

## Compile and flash

```bash
mkdir build
cd build
cmake -DPICO_BOARD=pico_w ..
make blink
```

Then enter BOOTSEL mode on the Pico W and copy the `build/blink.uf2` file to the mounted volume.
