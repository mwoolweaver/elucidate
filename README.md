# Elucidate

(ĭ-lo͞o′sĭ-dāt′) 

Clean up Elucubratus for use with Procursus on checkra1n with Cydia.

## Issues

**will only work in `cydia` after installing the `Procursus` bootstrap via https://odysseyra1n.com.**

### Elucubratus Packages

only `mobilesubstrate`, `cydia`, & their dependencies from [Elucubratus](https://apt.bingner.com) that aren't provided by Procursus.

  * `mobilesubstrate`
  
    * Depends: `com.saurik.substrate.safemode`
   
  * `cydia`
    
    * Depends: `cydia-lproj (>= 1.1.10)`, `org.thebigboss.repo.icons`
     
also includes `com.bingner.snappy` cause I'm not sure of the consequences of not having it on [checkra1n](https://checkra.in)
   
### Procursus Packages

 * hides `dummy packages` provided by [Procursus](https://github.com/ProcursusTeam/Procursus/blob/master/build_tools/make_dummy.sh).

   * A `dummy package` is used to help migration from other bootstraps. Safe to remove.
    
 * hides older version of `cydia` provided by [Procursus](https://github.com/ProcursusTeam/repo/blob/master/pool/main/iphoneos-arm64/1600/cydia_1.1.33_iphoneos-arm.deb)
    
   * `cydia` Version: 1.1.33
