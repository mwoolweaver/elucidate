# Elucidate

 (ĭ-lo͞o′sĭ-dāt′) 

Clean up Elucubratus, Procursus, & Odyssey repos to work together on checkra1n.

# Requirements

 * install `Procursus` via https://odysseyra1n.com

# Caveats

***will only work in `cydia`***    

***a fix for `zebra` is in the pipeline [#1464](https://github.com/zbrateam/Zebra/issues/1464#issuecomment-692360058)***

## Package Pins

### [Elucubratus Packages](https://github.com/mwoolweaver/elucidate/blob/master/etc/apt/preferences.d/_elucidate_elucubratus)

only show the following 

  * `mobilesubstrate`

    * Depends: `com.saurik.substrate.safemode`

  * `cydia`

    * Depends: `cydia-lproj (>= 1.1.10)`, `org.thebigboss.repo.icons`

  * `com.bingner.snappy` - cause I'm not sure of the consequences of not having it on [checkra1n](https://checkra.in)

### [Procursus Packages](https://github.com/mwoolweaver/elucidate/blob/master/etc/apt/preferences.d/_elucidate_procursus)

hide the following 

   * `dummy packages` 
      > [A `dummy package` is used to help migration from other bootstraps. Safe to remove.](https://github.com/ProcursusTeam/Procursus/blob/master/build_tools/make_dummy.sh)
  
   * `cydia` Version: [1.1.33](https://github.com/ProcursusTeam/repo/blob/master/pool/main/iphoneos-arm64/1600/cydia_1.1.33_iphoneos-arm.deb)
 
### [Odyssey Packages](https://github.com/mwoolweaver/elucidate/blob/master/etc/apt/preferences.d/_elucidate_odyssey)

hide the following 

 * `preferenceloader` - causes issues for me and others as well so hide to avoid them
 * `com.muirey03.libmryipc` - causes update loops for some reason. . .

## Using elucidate

 * add `https://elucidate.woolweaver.bid` to Cydia after successfully installing Procursus.

## Disclaimer

   **I provide no support for Procursus/Odysseyra1n migration.**
