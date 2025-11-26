# Roulingo

Hello!
Roulingo is a preprocessing and solving system for the
**transit-constraint recurring pickup and delivery problem** (TCRPDP)
based on [**answer set programming**](https://potassco.org) (ASP).

- [Installation](#installation)
- [Usage](#usage)
    - [Instance Construction](#instance-construction)
        - [CSV Conversion](#csv-conversion)
        - [Preprocessing](#preprocessing)
    - [Solver Invocation](#solver-invocation)

## Installation

…


## Usage

…

> [!TIP]
> Invoke `roulingo --help` for an overview of available sub-commands.

### Instance Construction

An **instance** is defined by the following facts:

- `node(X,T)` denotes a node `X` with transshipment cost `T` per unit.
- `vehicle(V,C)` denotes a vehicle `V` with capacity `C`.
- `availability(V,B,E)` denotes a period of availability for vehicle `V` beginning at date `B` and ending after date `E`.
- `arc(X,Y,V,C,D)` denotes an arc from node `X` to node `Y` for vehicle `V` with travel cost `C` and duration `D`.
- `month(M,B,E)` denotes a month `M` beginning at date `B` and ending after date `E`.
- `demand(I,X,Y,M,Q,R,F,T)` denotes a demand `I` with origin node `X`, destination node `Y`, month of availability `M`,
total quantity `Q`, revenue per unit delivered `R`, **minimum pickup frequency** `F`, and **maximum transit time** `T`.

> [!NOTE]
> Transshipment is not currently supported,
> and transshipment costs `T` for each node `node(X,T)` are ignored.

#### CSV Conversion

The facts …

#### Preprocessing

…

### Solver Invocation

…
