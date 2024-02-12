# pythoneda-external-artf/nixpkgs

Artifact for NixOS/nixpkgs

## How to declare it in your flake

Check the latest tag of this repository: https://github.com/pythoneda-external-artf-def/nixpkgs, and use it instead of the `[version]` placeholder below.

```nix
{
  description = "[..]";
  inputs = rec {
    [..]
    pythoneda-external-artf-nixpkgs = {
      [optional follows]
      url =
        "github:pythoneda-external-artf-def/nixpkgs/[version]";
    };
  };
  outputs = [..]
};
```

Should you use another PythonEDA modules, you might want to pin those also used by this project. The same applies to [https://nixos/nixpkgs](nixpkgs "nixpkgs") and [https://github.com/numtide/flake-utils](flake-utils "flake-utils").

The Nix flake is managed by the [https://github.com/pythoneda-external-artf-def/nixpkgs](nixpkgs "nixpkgs") definition repository.

Use the specific package depending on your system (one of `flake-utils.lib.defaultSystems`) and Python version:

- `#packages.[system].pythoneda-external-artf-nixpkgs-python38`
- `#packages.[system].pythoneda-external-artf-nixpkgs-python39`
- `#packages.[system].pythoneda-external-artf-nixpkgs-python310`
- `#packages.[system].pythoneda-external-artf-nixpkgs-python311`
