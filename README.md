# Batch Connect - OSC Abaqus/CAE

![GitHub Release](https://img.shields.io/github/release/osc/bc_osc_abaqus.svg)
![GitHub License](https://img.shields.io/github/license/osc/bc_osc_abaqus.svg)

A Batch Connect app designed for OSC OnDemand that launches Abaqus within an
**Owens batch job using software rendering**.

## Prerequisites

This app requires the following software be installed on the nodes that the
batch job is intended to run on:

- [Abaqus/CAE](https://www.3ds.com/products-services/simulia/products/abaqus/abaquscae/) 6.14+
- [Lmod](https://www.tacc.utexas.edu/research-development/tacc-projects/lmod) 6.0.1+
- [Fluxbox](http://fluxbox.org/) 1.1.1+

For VNC server support:

- [TurboVNC](http://www.turbovnc.org/) 2.1+
- [websockify](https://github.com/novnc/websockify) 0.8.0+

For hardware rendering support:

- This simple version does not demonstrate hardware rendering support.
  See https://github.com/OSC/bc_osc_abaqus for an example of this.

## Install

Use git to clone this app and checkout the desired branch/version you want to
use:

```sh
scl enable git19 -- git clone <repo>
cd <dir>
scl enable git19 -- git checkout <tag/branch>
```

You will not need to do anything beyond this as all necessary assets are
installed. You will also not need to restart this app as it isn't a Passenger
app.

To update the app you would:

```sh
cd <dir>
scl enable git19 -- git fetch
scl enable git19 -- git checkout <tag/branch>
```

Again, you do not need to restart the app as it isn't a Passenger app.

## Contributing

1. Fork it ( https://github.com/OSC/bc_osc_abaqus/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
