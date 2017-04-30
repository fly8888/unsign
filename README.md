codesign --remove-signature 在删除代码签名之后没有修复MachO Header的偏移，导致生成的MachO文件畸形。我很确定应该有无数人踩过这个坑，自己研究一遍权当练习

这个是修复版


http://www.iosre.com/t/codesign-bug/7833

[![Join the chat at https://gitter.im/unsign-mach-o/Lobby](https://badges.gitter.im/unsign-mach-o/Lobby.svg)](https://gitter.im/unsign-mach-o/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![ISC License](https://img.shields.io/badge/license-ISC%20License-blue.svg)](https://opensource.org/licenses/ISC)

### Building

    make

### Installing

1. `make`.
2. Move `unsign` to wherever you like.

### License
ISC

### Original

http://www.woodmann.com/collaborative/tools/index.php/Unsign

