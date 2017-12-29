# betaflight-tx-lua-basic
Basic set of scripts to configure Betaflight from your Taranis TX (OpenTx)

This is a simplied set of configuration 'lua' scripts, based on the v0.3 version of the '[betaflight-tx-lua-scripts](https://github.com/betaflight/betaflight-tx-lua-scripts)' repository.
The 'betaflight-tx-lua-scripts' repository now contains many more screens.  This version has only the "PIDs", "Rates" and "VTX" screens.

The VTX screen has the following enhancements:

* Can step through available frequencies for bands / channels. Implements feature suggested by issue [#33](https://github.com/betaflight/betaflight-tx-lua-scripts/issues/33).

* If Betaflight has 'SetFreqByMHzMsp' support then any frequency in MHz can be set (via band 'U'); see: http://www.etheli.com/CF/vtxCfgCMSFreqViaMsp

* When doing a 'save' on the VTX screen, now performs an EEPROM_SAVE after updating the values (needed for latest version of Betaflight).

* Shows 'Retrying' if save-retry happens.

See the [Releases page](https://github.com/ethomas997/betaflight-tx-lua-basic/releases) to install the scripts.