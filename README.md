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

only show the following, hide everything else

  * `mobilesubstrate` - a powerful code insertion platform
  
    depends
    
    * `com.saurik.substrate.safemode` - safe mode safety extension (safe)

  * `cydia` - a graphical iPhone front-end for APT
  
    depends

    * `cydia-lproj (>= 1.1.10)` - languages and translations for Cydia
    
    * `org.thebigboss.repo.icons` - locally cached package icons from BigBoss

  * `com.bingner.snappy` - A tool for APFS snapshot management

### [Procursus Packages](https://github.com/mwoolweaver/elucidate/blob/master/etc/apt/preferences.d/_elucidate_procursus)

only hide the following, show everything else

   * all `dummy packages` 
      > [a `dummy package` is used to help with migration from other bootstraps. Safe to remove.](https://github.com/ProcursusTeam/Procursus/blob/master/build_tools/make_dummy.sh#L5)
  
   * `cydia` Version: [1.1.33](https://github.com/ProcursusTeam/repo/blob/master/pool/main/iphoneos-arm64/1600/cydia_1.1.33_iphoneos-arm.deb) - since we can use the version from Elucubratus we don't need this one.
 
### [Odyssey Packages](https://github.com/mwoolweaver/elucidate/blob/master/etc/apt/preferences.d/_elucidate_odyssey)

only hide the following, show everything else

 * `preferenceloader` - causes issues for me and others as well so hide to avoid them.
 
 * `com.muirey03.libmryipc` - causes update loops cause it's outdated.

## Using elucidate

 * add `https://elucidate.woolweaver.bid` to Cydia after successfully installing Procursus.

## Disclaimer

   **I provide no support for Procursus/Odysseyra1n migration.**
