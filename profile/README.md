# Welcome to POX OS ⚡

<p align="center">
  <img src="https://avatars.githubusercontent.com/u/338706181?v=4" width="160" alt="POX OS" />
  <br>
  <b>A refined, modular, and aesthetic Android distribution based on LineageOS and AOSP.</b>
</p>

---

### ✨ Vision & Aesthetics
POX OS is designed from the ground up for users and developers who value:
- **Reinvented UI/UX**: Fluid system styling, custom lockscreens, dynamic quick settings, and deep palette theming.
- **Modular Customization**: A dedicated tweak dashboard ([POX Hub](https://github.com/pox-os/packages_apps_PoxHub)) that separates core system stability from aesthetic controls.
- **Rock-Solid Foundation**: Upstream stability tracking LineageOS and Google AOSP releases.

---

### 📦 Key Repositories
| Repository | Description |
| :--- | :--- |
| [manifest](https://github.com/pox-os/manifest) | The primary repo manifest to sync source trees |
| [vendor_pox](https://github.com/pox-os/vendor_pox) | Core makefiles, branding, bootanimations, and overlays |
| [frameworks_base](https://github.com/pox-os/frameworks_base) | Core framework, SystemUI, and aesthetic modifications |
| [packages_apps_Settings](https://github.com/pox-os/packages_apps_Settings) | Custom system settings dashboard and device info |
| [packages_apps_PoxHub](https://github.com/pox-os/packages_apps_PoxHub) | Dedicated ROM customization center |
| [build_make](https://github.com/pox-os/build_make) | Build system configurations and lunch targets |

---

### 🚀 Syncing the Source
```bash
repo init -u https://github.com/pox-os/manifest -b pox-15.0 --git-lfs
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j$(nproc --all)
```

---

<p align="center">
  Maintained by <a href="https://github.com/txorav">@txorav</a> & the POX OS Community.
</p>
