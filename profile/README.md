# Welcome to POX OS ⚡

<p align="center">
  <img src="https://avatars.githubusercontent.com/u/338706181?v=4" width="160" alt="POX OS Logo" />
  <br>
  <b>A Refined, Aesthetic Android Operating System Built on Pure AOSP.</b>
  <br>
  <i>Certified Architecture adhering to <a href="https://github.com/pitpitpo/devskill">DevSkill Standards</a> (Project Treble, Stable AIDL, GSI Ready)</i>
</p>

---

### 🏛️ Pure AOSP Foundation
Unlike traditional custom ROMs derived from intermediate distributions, **POX OS** is built directly from the official **Google Android Open Source Project (AOSP)** upstream (`android-15.0.0_r14` Vanilla Ice Cream):
- **Upstream Purity**: Syncs directly against `https://android.googlesource.com`.
- **Project Treble Segregation**: Strict separation between system framework and vendor HALs using Stable AIDL.
- **Generic System Image (GSI)**: Supports clean boot on Treble-compliant devices out of the box.

---

### 📦 Organization Repositories
| Repository | Description |
| :--- | :--- |
| [manifest](https://github.com/pox-os/manifest) | The primary repo manifest syncing pure Google AOSP + POX overrides |
| [vendor_pox](https://github.com/pox-os/vendor_pox) | AOSP product configurations (`AndroidProducts.mk`), versioning, overlays |
| [frameworks_base](https://github.com/pox-os/frameworks_base) | Core framework, SystemUI, and aesthetic modifications |
| [packages_apps_Settings](https://github.com/pox-os/packages_apps_Settings) | System settings dashboard and "About POX" device info |
| [packages_apps_PoxHub](https://github.com/pox-os/packages_apps_PoxHub) | Dedicated ROM customization center in `/system_ext` |
| [build_make](https://github.com/pox-os/build_make) | Build system configurations and lunch targets |

---

### 🚀 Syncing the Source
```bash
repo init -u https://github.com/pox-os/manifest -b pox-15.0 --git-lfs
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```

### 🔨 Building POX OS
```bash
source build/envsetup.sh
lunch pox_arm64-trunk_staging-userdebug
m pox
```

---

<p align="center">
  Maintained by <a href="https://github.com/txorav">@txorav</a> & the POX OS Community.
</p>
