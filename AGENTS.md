# PLC Project - Agent Documentation

## Project Overview
This is a TIA Portal V21 PLC project targeting S7-1500 hardware with VCI integration for automated compilation and testing.

## Build Commands
```powershell
# TIA Portal VCI Build (if configured)
# Use TIA Portal VCI command line tools for compilation
# tia-vc build --project "C:\Users\WTT\plc" --target "S7-1500"
```

## Test Commands
```powershell
# PLCSIM Testing (if configured)
# Use PLCSIM for simulation testing
# plcsim-start --project "C:\Users\WTT\plc" --runtime "S7-1500"
```

## Verification Steps
1. Check SCL syntax in `src/scl/` directories
2. Verify LAD/FBD documentation completeness
3. Validate data block structures in `docs/data_blocks/`
4. Confirm hardware configuration in `config/hardware/`
5. Test tag definitions in `config/tags/`

## Project Structure
- `src/scl/` - Structured Control Language source code
- `src/lad_fbd/` - Ladder Logic and Function Block Diagram documentation
- `docs/data_blocks/` - Data Block documentation
- `docs/plc_types/` - PLC data type definitions
- `config/tags/` - Tag definitions and naming conventions
- `config/hardware/` - Hardware configuration

## File Extensions
- `.scl` - SCL source files
- `.fb` - Function Block files
- `.ob` - Organization Block files
- `.lad` - Ladder Logic documentation
- `.fbd` - Function Block Diagram documentation
- `.db` - Data Block documentation
- `.udt` - User-Defined Type documentation
- `.tags` - Tag configuration files
- `.hw` - Hardware configuration files

## Target Platform
- PLC: S7-1500
- Software: TIA Portal V21
- Simulation: PLCSIM
- Integration: VCI (Virtual Control Interface)

## Development Workflow
1. Develop SCL code in appropriate directories
2. Document LAD/FBD logic
3. Define data blocks and types
4. Configure tags and hardware
5. Test in PLCSIM
6. Commit changes to repository
