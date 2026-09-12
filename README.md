# PLC Project - TIA Portal V21

This repository contains the PLC project structure for TIA Portal V21 development targeting S7-1500 PLCs.

## Project Structure

```
plc/
├── src/
│   ├── scl/                     # Structured Control Language source code
│   │   ├── functions/          # Individual function blocks (FC)
│   │   ├── function_blocks/    # Function blocks with memory (FB)
│   │   └── organization_blocks/ # OBs (Main, Startup, Error handling)
│   └── lad_fbd/                # Ladder Logic and Function Block Diagrams
│       ├── ladder_logic/       # LAD source documentation
│       └── function_block_diagrams/ # FBD source documentation
├── docs/
│   ├── data_blocks/            # Data Block documentation
│   │   ├── instance_dbs/       # Instance data blocks
│   │   └── shared_dbs/         # Shared data blocks
│   └── plc_types/              # PLC data type definitions
│       ├── udts/               # User-defined types
│       ├── arrays/             # Array definitions
│       └── structs/            # Structure definitions
├── config/
│   ├── tags/                   # Tag definitions and naming conventions
│   │   ├── io_tags/            # Input/Output tags
│   │   ├── memory_tags/        # Memory tags
│   │   └── system_tags/        # System tags
│   └── hardware/               # Hardware configuration
│       ├── plc_hardware/       # PLC hardware setup
│       └── network_config/     # Network configuration
└── README.md
```

## Development Workflow

1. **Clone Repository**: Clone this repository to your local development environment
2. **Open in TIA Portal**: Import the project structure into TIA Portal V21
3. **Development**: 
   - Write SCL code in `src/scl/` directories
   - Document LAD/FBD logic in `src/lad_fbd/` directories
   - Define data blocks in `docs/data_blocks/`
   - Configure tags in `config/tags/`
4. **Testing**: Use PLCSIM for simulation and testing
5. **Commit**: Push changes to GitHub for version control

## TIA Portal V21 VCI Integration

This project is designed to work with TIA Portal V21 VCI (Virtual Control Interface) for:
- Automated compilation
- Integration with CI/CD pipelines
- PLCSIM testing automation
- Version control integration

## Target Hardware

- **PLC**: S7-1500
- **Software**: TIA Portal V21
- **Simulation**: PLCSIM

## Conventions

- SCL files use `.scl` extension
- LAD documentation uses `.lad` extension
- FBD documentation uses `.fbd` extension
- Data blocks use `.db` extension
- Follow Siemens naming conventions for tags and blocks

## Getting Started

1. Install TIA Portal V21
2. Clone this repository
3. Open TIA Portal and create new project
4. Import the directory structure
5. Configure hardware in `config/hardware/`
6. Start developing your PLC logic

## Branching Strategy

- `main`: Production-ready code
- `develop`: Development branch
- `feature/*`: Feature-specific branches
- `bugfix/*`: Bug fix branches

## License

[Add your license here]

## Contact

For questions or support, please contact the development team.
