# ![radioconda](static/radioconda_logo_web.png)

**To install radioconda, visit https://github.com/radioconda/radioconda-installer.**

Radioconda is a collection of open source **software radio** packages bundled with the [conda](https://conda.io/) package manager, including

- Digital RF
- GNU Radio (including an increasing list of out-of-tree modules)
- gqrx
- inspectrum

and support for the following SDR devices and device libraries:

|                  Device                  |                    Library                    |
| :--------------------------------------: | :-------------------------------------------: |
|             [ADALM-PLUTO][1]             |       libiio ([setup](#iio-pluto-sdr))        |
|         [Airspy R2/Mini/HF+][2]          | airspy/airspyhf ([setup](#airspy-r2-mini-hf)) |
|               [BladeRF][3]               |          bladeRF ([setup](#bladerf))          |
|             [Ettus USRPs][4]             |        UHD ([setup](#uhd-ettus-usrp))         |
|       [Funcube Dongle Pro/Pro+][5]       |            SoapyFCDPP / gr-funcube            |
|               [HackRF][6]                |           HackRF ([setup](#hackrf))           |
|               [LimeSDR][7]               |        Lime Suite ([setup](#limesdr))         |
| [Mirics MSi001 + MSi2500 SDR devices][8] |        libmirisdr ([setup](#mirisdr))         |
|             [Red Pitaya][9]              |                SoapyRedPitaya                 |
|      [RFSpace/NetSDR/CloudSDR][10]       |                  SoapyNetSDR                  |
|              [RTL-SDR][11]               |          rtl-sdr ([setup](#rtl-sdr))          |
|        Sound Card / Audio devices        |                  SoapyAudio                   |

[1]: https://www.analog.com/en/design-center/evaluation-hardware-and-software/evaluation-boards-kits/adalm-pluto.html
[2]: https://airspy.com/
[3]: https://www.nuand.com/
[4]: https://www.ettus.com/products/
[5]: https://www.funcubedongle.com/
[6]: https://greatscottgadgets.com/hackrf/
[7]: https://limemicro.com/products/boards/
[8]: https://github.com/f4exb/libmirisdr-4
[9]: https://redpitaya.com/
[10]: http://www.rfspace.com/RFSPACE/Home.html
[11]: https://www.rtl-sdr.com/buy-rtl-sdr-dvb-t-dongles/

The complete list of packages can be found [here](https://github.com/radioconda/radioconda-installer/blob/master/radioconda.yaml). You can [**suggest additional software to include**](https://github.com/radioconda/radioconda-installer/issues) by filing an [issue](https://github.com/radioconda/radioconda-installer/issues). If you've built additional software from source on top of radioconda, [**document your results**](https://github.com/radioconda/radioconda-installer/issues) in an [issue](https://github.com/radioconda/radioconda-installer/issues) to help others (and help me in packaging it!).

Once installed, you will have a fully functional conda distribution/environment, meaning that you can use the `conda` or `mamba` commands to install additional packages (if available through [conda-forge](https://conda-forge.org/feedstock-outputs)) or upgrade to the latest versions. Think of radioconda as an alternative to [Anaconda](https://www.anaconda.com/products/individual) or [Miniforge](https://github.com/conda-forge/miniforge), but specialized for software radio.

**NOTE:** Radioconda is built from packages maintained by the [conda-forge](https://conda-forge.org/) project. If you have questions or issues that are specific to the conda installation of a particular package, please report them at the corresponding [feedstock repository](https://github.com/conda-forge/feedstocks).
