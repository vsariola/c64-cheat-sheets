# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).

## v0.3.0

### Added
- B flag is explained better in the footnote
- Added note about LAX and XAA being stable if the operand is 0
or the current accumulator value is 255
- I⇒1 added to the BRK function

### Fixed
- The pre- and post-increment symbols are used incorrectly (vice versa)
- BRK jumps indirectly, i.e. $FFFE⇒PC was changed to ($FFFE)⇒PC
- JSR pushes PC+2.
- RTS increments the address by 1 before transferring it to PC.
- One line was on a wrong layer
- BRK does not actually manipulate B flag (it's already 1. Only during IRQ/NMI
  is the B flag 0)

### Changed
- Distributed lines between addressing mode headers using equal gap, instead of
putting them between the centers of the titles
- "Decimal" -> "Decimal mode"
- The names of some of the unintended opcodes were changed to match more common
ones

## v0.2.0

### Added
- More illegals: illegal NOPs, JAMs and SBC2

### Changed
- Use only open source fonts: Jost and Noto Sans Math

## v0.1.0

### Added
- Initial version

[0.3.0]: https://github.com/vsariola/c64-cheat-sheets/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/vsariola/c64-cheat-sheets/compare/v0.1.0...v0.2.0
[0.1.0]: https://github.com/vsariola/c64-cheat-sheets/releases/tag/v0.1.0
