# Arduino NINA-W102 firmware

This firmware uses [Espressif's IDF](https://github.com/espressif/esp-idf)

## Building

1. [Download/Compile the ESP32 toolchain](https://docs.espressif.com/projects/esp-idf/en/v4.1/get-started/linux-setup-scratch.html)
1. Extract it and add it to your `PATH`: `export PATH=$PATH:<path/to/toolchain>/bin`
1. Clone **v4.3-dev** of the IDF: `git clone --branch v4.3-dev --recursive https://github.com/espressif/esp-idf.git`
1. Set the `IDF_PATH` environment variable: `export IDF_PATH=<path/to/idf>`
1. Install the necessary python dependencies `python -m pip install --user -r $IDF_PATH/requirements.txt`
1. Run `make` to build the firmware (in the directory of this read me)
1. Load the `Tools -> SerialNINAPassthrough` example sketch on to the board
1. Use `esptool` to flash the compiled firmware

## License

Copyright (c) 2018-2019 Arduino SA. All rights reserved.

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public
License along with this library; if not, write to the Free Software
Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA
